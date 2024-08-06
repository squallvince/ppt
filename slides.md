---
theme: seriph
background: https://assets.myportal.dev.porsche-preview.cn/pwsa-ui/assets/png/new-weapp-Dr9XSI79.png
title: CAT前端发展史
class: text-center
highlighter: shiki
themeConfig:
  primary: '#fff'
drawings:
  persist: false
transition: slide-left
mdc: true
---

# CAT前端发展史

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    进入下一页 <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:edit />
  </button>
  <a href="https://github.com/slidevjs/slidev" target="_blank" alt="GitHub" title="Open in GitHub"
    class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

---

# 为什么要做彻底的重构

清晰的架构设计，提升项目可维护性、可扩展性、可测试性、可复用性

- 📝 **ReadMe** - 专注Markdown描述，让项目清晰易懂
- 🎨 **Themable** - 可共享的主题并提供在线加载能力
- 🧑‍💻 **Developer Friendly** - 代码提示，保存自动格式化
- 🚀 **High Efficiency** - 极速本地启动，线上两分钟部署
- 🌿 **Dispersed** - 按需加载，文件体积小

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

# 曾经的CAT

|                                                    |                             |                             |
| -------------------------------------------------- | --------------------------- | --------------------------- |
| <kbd>PWSA</kbd>                                    | react 16.8.2     |  js体积：8.5M     |
| <kbd>RSA</kbd>                                     | react 16.8.2     |  js体积：2M     |
| <kbd>SR</kbd>                                      | react 16.8.2     |  js体积：2.4M     |
| <kbd>SAB</kbd>                                     | angular 8.2      |  js体积：30M     |
| <kbd>PD</kbd>                                      | angular 8.2      |  js体积： 30M    |

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

# 现在的CAT


<div v-click> 猜猜现在PWSA的JS总体积多大？ </div>
<div class="flex-container" style="display: flex;">
  <div class="flex-item m-10" v-click> 3M </div>
  <div v-click class="flex-item" style="width: 50%;"><img src="https://www.douyin766.com/wp-content/uploads/2020/07-29/faa7604a643234d9f93a1509491838a7.png" alt="what?" /></div>
</div>

<!-- Inline style -->
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

# 驱动力：变得更好

<div class="flex-container" style="display: flex;">
  <div class="flex-item pr-10">
    <p>- CDN</p>
    <p>- ESModule</p>
    <p>- Gzip或Br压缩</p>
    <p>- 懒加载</p>
  </div>
  <div class="flex-item" style="width: 50%;"><img src="https://s3.cn-north-1.jdcloud-oss.com/shendengbucket1/2023-03-29-11-33eeDHeG28Xb0n33jvb.png" alt="驱动力" /></div>
</div>

<!-- Inline style -->
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

# GitLab

[Documentations](https://gitlab.porsche-preview.cn/porsche-digital-china/myporsche/mycat-web-pwsa)

<!-- Inline style -->
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

