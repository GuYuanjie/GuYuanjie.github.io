---
title: "Gallery"
description: "Capturing moments, pixels, and light."
layout: "simple"
showTableOfContents: true
---

{{< lead >}}
这里的每一张照片都是时间的切片。
<br>
无论是**街头摄影**、**数字艺术**还是我的**桌面搭配**，我喜欢用视觉语言记录生活。
{{< /lead >}}

<!-- 
  分类筛选器 (锚点导航)
  点击可快速跳转到对应区域
-->
<div class="flex flex-wrap gap-3 justify-center mb-10">
  <a href="#-photography" class="px-4 py-1.5 rounded-full bg-neutral-100 dark:bg-neutral-800 hover:bg-primary-100 dark:hover:bg-primary-900 text-neutral-700 dark:text-neutral-300 transition-colors text-sm font-medium no-underline">
    📸 Photography
  </a>
  <a href="#-digital-art" class="px-4 py-1.5 rounded-full bg-neutral-100 dark:bg-neutral-800 hover:bg-primary-100 dark:hover:bg-primary-900 text-neutral-700 dark:text-neutral-300 transition-colors text-sm font-medium no-underline">
    🎨 Digital Art
  </a>
  <a href="#-battlestation" class="px-4 py-1.5 rounded-full bg-neutral-100 dark:bg-neutral-800 hover:bg-primary-100 dark:hover:bg-primary-900 text-neutral-700 dark:text-neutral-300 transition-colors text-sm font-medium no-underline">
    🖥️ Battlestation
  </a>
</div>

---

## 📸 Photography

这里使用了 **Blowfish 的 Gallery Shortcode**。图片会自动排版并支持点击放大。

<!-- 
  使用 gallery 短代码
  注意：请将图片替换为你 static/images/ 目录下的真实图片
-->
{{< gallery >}}
  <img src="https://images.unsplash.com/photo-1492691527719-9d1e07e534b4?ixlib=rb-1.2.1&auto=format&fit=crop&w=1000&q=80" class="grid-w33" alt="Mountains" />
  <img src="https://images.unsplash.com/photo-1470770841072-f978cf4d019e?ixlib=rb-1.2.1&auto=format&fit=crop&w=1000&q=80" class="grid-w33" alt="Landscape" />
  <img src="https://images.unsplash.com/photo-1433838552652-f9a46b332c40?ixlib=rb-1.2.1&auto=format&fit=crop&w=1000&q=80" class="grid-w33" alt="Nature" />
  <img src="https://images.unsplash.com/photo-1441974231531-c6227db76b6e?ixlib=rb-1.2.1&auto=format&fit=crop&w=1000&q=80" class="grid-w50" alt="Forest" />
  <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?ixlib=rb-1.2.1&auto=format&fit=crop&w=1000&q=80" class="grid-w50" alt="Waterfall" />
{{< /gallery >}}

---

## 🎨 Digital Art

这里使用了 **CSS Columns (Masonry)** 布局，适合展示长宽比不一的图片（如 AI 生成的竖图）。鼠标悬停时会显示详细信息。

<div class="columns-1 md:columns-2 lg:columns-3 gap-4 space-y-4">

  <!-- 图片卡片 1 -->
  <div class="break-inside-avoid group relative rounded-xl overflow-hidden cursor-pointer">
    <img src="https://images.unsplash.com/photo-1620641788421-7a1c342ea42e?auto=format&fit=crop&w=800&q=80" class="w-full h-auto object-cover transform transition-transform duration-500 group-hover:scale-110" alt="Art 1">
    <!-- 悬停遮罩 -->
    <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-transparent to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex flex-col justify-end p-4">
      <span class="text-white font-bold text-sm">Cyberpunk City</span>
      <span class="text-neutral-300 text-xs font-mono mt-1">Midjourney v6 • --ar 9:16</span>
    </div>
  </div>

  <!-- 图片卡片 2 -->
  <div class="break-inside-avoid group relative rounded-xl overflow-hidden cursor-pointer">
    <img src="https://images.unsplash.com/photo-1635322966219-b75ed372eb01?auto=format&fit=crop&w=800&q=80" class="w-full h-auto object-cover transform transition-transform duration-500 group-hover:scale-110" alt="Art 2">
    <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-transparent to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex flex-col justify-end p-4">
      <span class="text-white font-bold text-sm">Neon Dreams</span>
      <span class="text-neutral-300 text-xs font-mono mt-1">Stable Diffusion</span>
    </div>
  </div>

  <!-- 图片卡片 3 -->
  <div class="break-inside-avoid group relative rounded-xl overflow-hidden cursor-pointer">
    <img src="https://images.unsplash.com/photo-1550684848-fac1c5b4e853?auto=format&fit=crop&w=800&q=80" class="w-full h-auto object-cover transform transition-transform duration-500 group-hover:scale-110" alt="Art 3">
    <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-transparent to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex flex-col justify-end p-4">
      <span class="text-white font-bold text-sm">Abstract Flow</span>
      <span class="text-neutral-300 text-xs font-mono mt-1">DALL-E 3</span>
    </div>
  </div>

</div>

---

## 🖥️ Battlestation

使用 **Carousel (轮播)** 来展示同一个主题的不同角度。

{{< carousel images="https://images.unsplash.com/photo-1498050108023-c5249f4df085, https://images.unsplash.com/photo-1504639725590-34d0984388bd, https://images.unsplash.com/photo-1555066931-4365d14bab8c" >}}

---

## 🎞️ Photo Log (Polaroid Style)

一种拍立得风格的布局，带有 EXIF 数据，适合记录旅行故事。

<div class="grid grid-cols-1 md:grid-cols-2 gap-8 mt-8">

  <!-- 拍立得卡片 1 -->
  <div class="bg-white dark:bg-neutral-800 p-3 pb-4 rounded-sm shadow-md rotate-1 hover:rotate-0 transition-transform duration-300 border border-neutral-100 dark:border-neutral-700">
    <div class="overflow-hidden aspect-[4/3] mb-3 relative group">
      <img src="https://images.unsplash.com/photo-1516483638261-f4dbaf036963" class="w-full h-full object-cover">
      <!-- EXIF 标签 -->
      <div class="absolute bottom-2 right-2 bg-black/60 backdrop-blur-sm text-white text-[10px] px-2 py-1 rounded font-mono opacity-0 group-hover:opacity-100 transition-opacity">
        ISO 100 • f/2.8 • 1/200s
      </div>
    </div>
    <div class="px-1 text-center">
      <p class="font-handwriting text-xl text-neutral-800 dark:text-neutral-200">Cinque Terre, Italy</p>
      <p class="text-xs text-neutral-400 mt-1 uppercase tracking-widest">Summer 2024</p>
    </div>
  </div>

  <!-- 拍立得卡片 2 -->
  <div class="bg-white dark:bg-neutral-800 p-3 pb-4 rounded-sm shadow-md -rotate-1 hover:rotate-0 transition-transform duration-300 border border-neutral-100 dark:border-neutral-700">
    <div class="overflow-hidden aspect-[4/3] mb-3 relative group">
      <img src="https://images.unsplash.com/photo-1477959858617-67f85cf4f1df" class="w-full h-full object-cover">
      <div class="absolute bottom-2 right-2 bg-black/60 backdrop-blur-sm text-white text-[10px] px-2 py-1 rounded font-mono opacity-0 group-hover:opacity-100 transition-opacity">
        ISO 400 • f/1.8 • 1/60s
      </div>
    </div>
    <div class="px-1 text-center">
      <p class="font-handwriting text-xl text-neutral-800 dark:text-neutral-200">Urban Night</p>
      <p class="text-xs text-neutral-400 mt-1 uppercase tracking-widest">Chicago</p>
    </div>
  </div>

</div>
