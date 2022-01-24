# How to deploy a react application created on vitejs

- Create a repository on github
- Add the base property to the vite configurations and asign it your repository name 

``` javascript
  export default defineConfig({
  base: '/your-repository-name/' //Here add base property,
  plugins: [react()]
})

```
