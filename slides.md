---
theme: default
background: https://images.unsplash.com/photo-1518098177606-8e35400d3a2d?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2075&q=80
class: 'text-center'
highlighter: shiki
lineNumbers: false
drawings:
  persist: false
css: unocss
---

# Migrating CRA to Vite 

Pros and cons compilation of this change

---

# Why Vite?
Next generation frontend tooling. It's fast!

<br>

- 🌠 **Faster** - 10-100x faster dev server than Webpack
- 🧩 **Transpiling is done on-demand** - Makes code-splitting a priority

<br>
<br>

<img src="https://media.tenor.com/jD4sqQ5G6hIAAAAj/sonic-running.gif">

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(166deg, #4EC5D4 10%, #ca5cdd 20%);
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}

img {
  height: 80px;
  margin: auto 24px auto auto;
}
</style>

---
layout: center
class: text-center
---

# Esbuild vs Webpack
<img src="https://miro.medium.com/max/1400/0*xWW-OIn-CnQnt5jp" />

<style>
h1 {
  color: #4EC5D4;
}
</style>

---
---

# Pros and Cons
It has no cons (jokes)

<br>
<br>

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(166deg, #4EC5D4 10%, #ca5cdd 20%);
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---
---

# Pros and Cons
It has no cons (jokes)

<br>

<div class="grid grid-cols-2 gap-10 pt-4 -mb-6">

<div>

## Pros
<br>

- 🏃 Fast
- ⚙️ Easy to configure

</div>

<br>
<br>
</div>

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(166deg, #4EC5D4 10%, #ca5cdd 20%);
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}

h2 {
  color: #ca5cdd;
}
</style>

---
---

# Pros and Cons
It has no cons (jokes)

<br>

<div class="grid grid-cols-2 gap-10 pt-4 -mb-6">

<div>

## Pros
<br>

- 🏃 Fast
- ⚙️ Easy to configure

</div>

<div>

## Cons
<br>

- 🧑🏻‍💻 Can only target modern browsers (ES2015+)
- 🤷 It's just fast

</div>

<br>
<br>
</div>

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(166deg, #4EC5D4 10%, #ca5cdd 20%);
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}

h2 {
  color: #ca5cdd;
}
</style>

---
---

# How to migrate it

1. Install dependencies 

2. Create Vite config file

3. Update `index.html` paths

```html
  // before
    <link rel="manifest" href="%PUBLIC_URL%/manifest.json" />
    <link rel="shortcut icon" href="%PUBLIC_URL%/favicon.ico" />
  
  // after
        <link rel="manifest" href="/manifest.json" />
    <link rel="shortcut icon" href="/favicon.ico" />
```
<br>

4. Remove `react-scripts`

5. Update scripts in `package.json`

<style>
h1 {
  color: #ca5cdd;
}
</style>

---
layout: center
class: text-center
---

# My experience

<img src="https://www.icegif.com/wp-content/uploads/baby-yoda-icegif-2.gif" />


<style>
h1 {
  color: #4EC5D4;
}
</style>

---
---

# References

- [Vite 3.0 vs. Create React App: Comparison and migration guide](https://blog.logrocket.com/vite-3-vs-create-react-app-comparison-migration-guide/);
- [Migrating from Create React App (CRA) to Vite](https://cathalmacdonnacha.com/migrating-from-create-react-app-cra-to-vite);
- [Blazing fast TypeScript with Webpack and ESBuild](https://dev.to/karanpratapsingh/blazing-fast-typescript-with-webpack-and-esbuild-4mhh);
- [Has Vite Made Vue CLI Obsolete?](https://vuejsdevelopers.com/2020/12/07/vite-vue-cli/);
- [Why Vite (from Vite Doc)](https://vitejs.dev/guide/why.html);

<style>
h1 {
  color: #ca5cdd;
}

a:hover {
  color: #954f94;
}
</style>