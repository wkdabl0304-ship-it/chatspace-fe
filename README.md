# chatspace-fe

ChatSpace：仿微信即时聊天系统的 Vue 3 前端仓库

## 规范要求

1.函数名使用驼峰命名法，例如：handleLogin()

2.变量名使用下划线命名法，例如：modal_is_open

3.常量全大写，例如：AVERAGE_SCORE

4.参数不要写死在代码里，尽可能可配置，拓展时改动配置即可，而无需修改代码，比如前端页面端口、后端地址、枚举、数组等等

5.每个组件/页面/模块/函数等都要在开头写注释，其他详细注释看个人习惯，代码尽可能易于阅读，不要东一块西一块

6.不能改动 main 分支，在 develop 分支开发，每完成一部分完整的组件或小功能就 commit 分支，完成页面或大功能就请求合并到 main 分支，我再审核一遍

7.合并请求前需要先执行 npm run format 和 npm run lint，然后再请求合并

8.commit 和 merge 规范参考后端仓库，要能知道“做了什么事情”

9.包管理工具统一用 node.js 的 npm，不要用 pnpm

10.项目配置：TypeScript、Router、Pinia、ESLint、Prettier、Vitest、Playwright

11.95%+的问题询问 AI 可以解决，实在有疑问可以问我

以下为项目启动以及一些相关操作的说明文档：

This template should help get you started developing with Vue 3 in Vite.

## Recommended IDE Setup

[VS Code](https://code.visualstudio.com/) + [Vue (Official)](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur).

## Recommended Browser Setup

- Chromium-based browsers (Chrome, Edge, Brave, etc.):
  - [Vue.js devtools](https://chromewebstore.google.com/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd) 
  - [Turn on Custom Object Formatter in Chrome DevTools](http://bit.ly/object-formatters)
- Firefox:
  - [Vue.js devtools](https://addons.mozilla.org/en-US/firefox/addon/vue-js-devtools/)
  - [Turn on Custom Object Formatter in Firefox DevTools](https://fxdx.dev/firefox-devtools-custom-object-formatters/)

## Type Support for `.vue` Imports in TS

TypeScript cannot handle type information for `.vue` imports by default, so we replace the `tsc` CLI with `vue-tsc` for type checking. In editors, we need [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) to make the TypeScript language service aware of `.vue` types.

## Customize configuration

See [Vite Configuration Reference](https://vite.dev/config/).

## Project Setup

```sh
npm install
```

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Type-Check, Compile and Minify for Production

```sh
npm run build
```

### Run Unit Tests with [Vitest](https://vitest.dev/)

```sh
npm run test:unit
```

### Run End-to-End Tests with [Playwright](https://playwright.dev)

```sh
# Install browsers for the first run
npx playwright install

# When testing on CI, must build the project first
npm run build

# Runs the end-to-end tests
npm run test:e2e
# Runs the tests only on Chromium
npm run test:e2e -- --project=chromium
# Runs the tests of a specific file
npm run test:e2e -- tests/example.spec.ts
# Runs the tests in debug mode
npm run test:e2e -- --debug
```

### Lint with [ESLint](https://eslint.org/)

```sh
npm run lint
```
