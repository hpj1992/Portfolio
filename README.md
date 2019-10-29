# Static Personal Site

#### Components
- Developed using [Hugo](https://gohugo.io/)
- Using open sourced [themes](https://github.com/rhazdon/hugo-theme-hello-friend-ng)

#### Current Setup
- Hugo code at [Portfolio](https://github.com/hpj1992/Portfolio)
- Hugo Code + HTML Code at [harshit_site](https://github.com/hpj1992/harshit_site)
- HTML code for Github Hosting at [hpj1992.github.io](https://github.com/hpj1992/hpj1992.github.io)


#### Deployment Steps
- Checkout [Portfolio](https://github.com/hpj1992/Portfolio)
- Make Changes locally
- Test using [standard hugo practices](https://gohugo.io/getting-started/quick-start/)
- Checkout [harshit_site](https://github.com/hpj1992/harshit_site) to a directory (Reuse the same directory if already exists)
- Add `Public` folder and mark it as a submodule inside `harshit_site` for `hpj1992.github.io`
 - `git submodule add https://github.com/hpj1992/hpj1992.github.io.git public`
- [harshit_site](https://github.com/hpj1992/harshit_site) already has a file with correct commands for deployment `deploy.sh`
- Execute `./deploy.sh <commit-name-based-on-change>` from [harshit_site](https://github.com/hpj1992/harshit_site)
- Above deploy.sh execute will: 
  - Build html code from hugo site and put it inside `Public` folder
  - Github pages hosting requres index.html and other set of config which is handed by Hugo already
  - Push that change to a repo [hpj1992.github.io](https://github.com/hpj1992/hpj1992.github.io)
  - Once done, you can see your changes on internet - http://hpj1992.github.io
- At this point, it is still good idea to push these new changes to [harshit_site](https://github.com/hpj1992/harshit_site)
- To do that, go to root of [harshit_site](https://github.com/hpj1992/harshit_site) and push everything to Github
