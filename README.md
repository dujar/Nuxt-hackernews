# Project NUXT/VUE

Tutorial followed from John Lindquist using Nuxt as a dependency.
It is a server side rendering application that provides hacker news in a formatted way with atomic css with Tachyon.

# Hacker news website:
Thanks to the [hacker news API](https://github.com/HackerNews/API) 5 pages are rendered

- jobs
- top
- ask
- show
- new

# link

click [here]()

# What I have learned

Vue files, Nuxt structure with automatic code splitting, server side rendering. Routing structure with static file serving.

## nux.config.js

Configuration to incorporate features in the nuxt project.
Easy set up with Nuxt dependency that automatically  provides a server-rendered Vue.js application the same way as Next.js.


## vuex

store :

- state
- mutation
- actions

## plugins

- axios
- filters

## recursive components

recursively reuse the same component:comments  with the same component and v-for as the parent level component.

## css

the newly grid columns and row set up. Thanks to [css-trick](https://css-tricks.com/snippets/css/complete-guide-grid/)


## Build Setup

``` bash
# install dependencies
$ npm install # Or yarn install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, checkout the [Nuxt.js docs](https://github.com/nuxt/nuxt.js).
