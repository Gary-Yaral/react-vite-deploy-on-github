# How to deploy a react application created on vitejs

- Create a repository
- Add the called property base to the file vite.config and assign it your repository name.
 
``` javascript
  export default defineConfig({
  base: '/your-repository-name/' //Add base property here,
  plugins: [react()]
})

```
- Add the changes to the master or main branch
- Execute **npm run build**
- Next step
``` console
  git add dist -f
  git commit -m 'your commit'
  git subtree push --prefix dist origin gh-pages

```
