# How to deploy a react application created on vitejs

- Create a repository on github
- Add the called property base to the file vite.config and asign it your repository name. 

``` javascript
  export default defineConfig({
  base: '/your-repository-name/' //Add base property here,
  plugins: [react()]
})

```
- Add change to the master or main branch
- Execute **npm run build**
- Next step
``` console
  git add dist -f
  git commit -m 'your commit'
  git subtree push --prefix dist origin gh-pages

```
