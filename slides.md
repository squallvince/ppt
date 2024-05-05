---
theme: seriph
background: https://source.unsplash.com/collection/94734566/1920x1080
class: text-center
highlighter: shikiji
lineNumbers: false
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
drawings:
  persist: false
transition: slide-left
title: Qwik介绍与思考
mdc: true
---

# Qwik介绍与思考

---
transition: fade-out
---

# 前提知识：SSR

```html
<!DOCTYPE html>
<head>
  <title>SSR</title>
</head>
<body>
  <div id="SSR">
    <button>Hello!</button>
    <ul>
      <li>1</li>
      <li>2</li>
    </ul>
  </div>
  <script src="/main.js" defer></script>
</body>
```
<p v-after class="absolute bottom-40 left-45 opacity-30 transform -rotate-20">hydration</p>
---

# SSR流程有什么可优化的点?

感觉SSR可能是个"视觉骗子"

- 首屏展示的速度快了, 但是不可交互, 所以tti(页面可交互时间)并没有太大的优化。
- 仍然需要下载比较全量的js代码。
- js代码执行的时候, 仍然需要处理大量的逻辑, 还要重新处理一遍页面上的dom。

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---
layout: default
---

# Qwik是什么?

语法接近REACT的前端SSR框架

- 即时加载
- 可恢复
- 延迟执行
- 减少渲染
- 可扩展的性能
- 一次编码


<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---
layout: default
---

# 即时加载

<img src="https://cdn.builder.io/api/v1/image/assets%2Ffe30f73e01ef40558cd69a9493eba2a2%2Ffdc08238cb4d49d48d3a468308992e15" style="object-fit: contain;object-position: left center;position: absolute;height: 50%;width: 50%;top: 20%;left: 5%;background-color: #000;" role="presentation" loading="lazy">

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---

# 可恢复

<img src="https://cdn.builder.io/api/v1/image/assets%2Ffe30f73e01ef40558cd69a9493eba2a2%2Feee9dff8ee0e4b4e9ad1a8825643030c" style="object-fit: contain;object-position: left center;position: absolute;height: 50%;width: 50%;top: 20%;left: 5%;background-color: #000;" role="presentation" loading="lazy">

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---

# 延迟执行

<img src="https://cdn.builder.io/api/v1/image/assets%2Ffe30f73e01ef40558cd69a9493eba2a2%2F8f2ccdcaa669452c85c1b74d2c162a3d" style="object-fit: contain;object-position: left center;position: absolute;height: 50%;width: 50%;top: 20%;left: 5%;background-color: #000;" role="presentation" loading="lazy">

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---

# 减少渲染

<img src="https://cdn.builder.io/api/v1/image/assets%2Ffe30f73e01ef40558cd69a9493eba2a2%2Fefcf8d0391fe4d8bb7e557e6d295a2b2" style="object-fit: contain;object-position: left center;position: absolute;height: 50%;width: 50%;top: 20%;left: 5%;background-color: #000;" role="presentation" loading="lazy">

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---

# 可扩展的性能

<img src="https://cdn.builder.io/api/v1/image/assets%2Ffe30f73e01ef40558cd69a9493eba2a2%2F644d27976d234ec9b453501c209bffa3" style="object-fit: contain;object-position: left center;position: absolute;height: 50%;width: 50%;top: 20%;left: 5%;background-color: #000;" role="presentation" loading="lazy">

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---

# 一次编码

<img src="https://cdn.builder.io/api/v1/image/assets%2Ffe30f73e01ef40558cd69a9493eba2a2%2Fd805a18ff6d0410f92603fb691c87349" style="object-fit: contain;object-position: left center;position: absolute;height: 50%;width: 50%;top: 20%;left: 5%;background-color: #000;" role="presentation" loading="lazy">

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---

# 目录结构

```
qwik-app-demo
├── README.md
├── package.json
├── public
│   └── favicon.svg
├── src
│   ├── components
│   │   └── router-head
│   │       └── router-head.tsx
│   ├── entry.ssr.tsx
│   ├── global.css
│   ├── root.tsx
│   └── routes
│       ├── flower
│       │   ├── flower.css
│       │   └── index.tsx
│       ├── index.tsx
│       ├── layout.tsx
│       └── service-worker.ts
├── tsconfig.json
└── vite.config.ts
```
<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---

# 生命周期

```
useTask$ -------> RENDER ---> useVisibleTask$
                            |
| --- SERVER or BROWSER --- | ----- BROWSER ----- |
                            |
                       pause|resume
```
<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---

# Hook规则

```
useHook(); // <-- ❌ does not work
 
export default component$(() => {
  useCustomHook(); // <-- ✅ does work
  if (condition) {
    useHook(); // <-- ❌ does not work
  }
  useTask$(() => {
    useNavigate(); // <-- ❌ does not work
  });
  const myQrl = $(() => useHook()); // <-- ❌ does not work
  return <button onClick$={() => useHook()}></button>; // <-- ❌ does not work
});
 
function useCustomHook() {
  useHook(); // <-- ✅ does work
  if (condition) {
    useHook(); // <-- ❌ does not work
  }
}

```
<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---

layout: center
class: text-center
---

# Learn More

[Documentations](https://qwik.builder.io/)
