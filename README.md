# [Vue JS 2] README
> SKILL : `vue.js v2.x`, `BootstrapVue`
> <br>
> Vue 2 Docs : [Vue 2 Docs](https://v2.vuejs.org)
> <br>
> Bootstrap Vue Docs : [Bootstrap Vue Docs](https://bootstrap-vue.org/docs)
> <br>
> YouTube Class: [개발자의품격](https://youtu.be/sqH0u8wN4Rs)

## Vue 설치 및 프로젝트 생성

### Vue2 CLI 설치

```bash
➜ npm install -g @vue/cli

```

### Vue 프로젝트 생성
```bash
➜ vue create vue2-beginner
?  Your connection to the default yarn registry seems to be slow.
   Use https://registry.npmmirror.com for faster installation? Yes


Vue CLI v5.0.6
? Please pick a preset: Default ([Vue 2] babel, eslint)
? Pick the package manager to use when installing dependencies: NPM


Vue CLI v5.0.6
✨  Creating project in ../vue2-beginner.
🗃  Initializing git repository...
⚙️  Installing CLI plugins. This might take a while...


added 843 packages in 1m
🚀  Invoking generators...
📦  Installing additional dependencies...


added 83 packages in 10s
⚓  Running completion hooks...

📄  Generating README.md...

🎉  Successfully created project vue2-beginner.
👉  Get started with the following commands:

 $ cd vue2-beginner
 $ npm run serve

➜ 

```

### Vue Router 설치
vue3가 나온 시점에 vue2를 학습하고 있다보니 vue router 설치시 `vue-router@3`로 해줘야한다.
```bash
➜ npm install vue-router --save
또는
➜ npm install vue-router@3
```

### Bootstrap Vue 설치
[설치 참고](https://bootstrap-vue.org/docs#using-module-bundlers)
```bash
➜ npm install vue bootstrap bootstrap-vue
```



# vue2-beginner

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
