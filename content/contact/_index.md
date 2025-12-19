---
title: "Contact"
description: "Let's build something together."
layout: "simple"
showTableOfContents: false
---

{{< lead >}}
无论是讨论技术、寻求合作，还是只是想打个招呼，我都乐意倾听。
<br>
通常我会在 **24 小时内** 回复邮件。
{{< /lead >}}

<!-- 
  主要布局：双栏设计
  左侧：联系方式 & 状态
  右侧：联系表单
-->
<div class="grid grid-cols-1 md:grid-cols-2 gap-12 mt-8">

  <!-- LEFT COLUMN: Contact Info -->
  <div class="flex flex-col space-y-8">
    
    <!-- 1. Email Card (带有点击复制功能) -->
    <div class="p-6 rounded-2xl bg-neutral-50 dark:bg-neutral-800 border border-neutral-100 dark:border-neutral-700">
      <div class="flex items-center gap-3 mb-2">
        <span class="p-2 rounded-full bg-primary-100 text-primary-600 dark:bg-primary-900 dark:text-primary-300">
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect width="20" height="16" x="2" y="4" rx="2"/><path d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7"/></svg>
        </span>
        <h3 class="font-bold text-lg">Email</h3>
      </div>
      <p class="text-neutral-500 dark:text-neutral-400 text-sm mb-4">
        这是联系我最快的方式。
      </p>
      
      <!-- Copy Button -->
      <div class="relative group cursor-pointer" onclick="copyEmail(this)">
        <div class="flex items-center justify-between p-3 rounded-lg bg-white dark:bg-neutral-900 border border-neutral-200 dark:border-neutral-700 hover:border-primary-500 transition-colors">
          <code id="email-text" class="font-mono text-neutral-800 dark:text-neutral-200">your.email@example.com</code>
          <span class="text-neutral-400 group-hover:text-primary-500 transition-colors">
            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect width="14" height="14" x="8" y="8" rx="2" ry="2"/><path d="M4 16c-1.1 0-2-.9-2-2V4c0-1.1.9-2 2-2h10c1.1 0 2 .9 2 2"/></svg>
          </span>
        </div>
        <!-- Tooltip -->
        <span class="absolute -top-8 left-1/2 -translate-x-1/2 bg-black text-white text-xs py-1 px-2 rounded opacity-0 group-hover:opacity-100 transition-opacity pointer-events-none">Click to Copy</span>
      </div>
    </div>

    <!-- 2. Social Links Grid -->
    <div>
      <h3 class="font-bold text-lg mb-4">On the Web</h3>
      <div class="grid grid-cols-2 gap-3">
        <a href="https://github.com/GuYuanjie" target="_blank" class="flex items-center gap-3 p-3 rounded-xl hover:bg-neutral-50 dark:hover:bg-neutral-800 border border-transparent hover:border-neutral-200 dark:hover:border-neutral-700 transition-all">
          <span class="text-2xl">🐙</span>
          <div>
            <div class="font-medium text-sm">GitHub</div>
            <div class="text-xs text-neutral-500">Follow my code</div>
          </div>
        </a>
        <a href="https://twitter.com" target="_blank" class="flex items-center gap-3 p-3 rounded-xl hover:bg-neutral-50 dark:hover:bg-neutral-800 border border-transparent hover:border-neutral-200 dark:hover:border-neutral-700 transition-all">
          <span class="text-2xl">🐦</span>
          <div>
            <div class="font-medium text-sm">Twitter</div>
            <div class="text-xs text-neutral-500">Daily thoughts</div>
          </div>
        </a>
        <a href="https://linkedin.com" target="_blank" class="flex items-center gap-3 p-3 rounded-xl hover:bg-neutral-50 dark:hover:bg-neutral-800 border border-transparent hover:border-neutral-200 dark:hover:border-neutral-700 transition-all">
          <span class="text-2xl">💼</span>
          <div>
            <div class="font-medium text-sm">LinkedIn</div>
            <div class="text-xs text-neutral-500">Resume & Connect</div>
          </div>
        </a>
        <a href="/index.xml" target="_blank" class="flex items-center gap-3 p-3 rounded-xl hover:bg-neutral-50 dark:hover:bg-neutral-800 border border-transparent hover:border-neutral-200 dark:hover:border-neutral-700 transition-all">
          <span class="text-2xl">📡</span>
          <div>
            <div class="font-medium text-sm">RSS</div>
            <div class="text-xs text-neutral-500">Subscribe</div>
          </div>
        </a>
      </div>
    </div>

    <!-- 3. Availability Status -->
    <div class="p-4 rounded-xl bg-green-50 dark:bg-green-900/20 border border-green-100 dark:border-green-800/30 flex items-start gap-3">
      <span class="relative flex h-3 w-3 mt-1.5">
        <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-green-400 opacity-75"></span>
        <span class="relative inline-flex rounded-full h-3 w-3 bg-green-500"></span>
      </span>
      <div>
        <h4 class="text-sm font-bold text-green-800 dark:text-green-300">Open for Opportunities</h4>
        <p class="text-xs text-green-700 dark:text-green-400 mt-1">目前我正在寻找全职工作或有趣的开源项目合作。</p>
      </div>
    </div>

  </div>

  <!-- RIGHT COLUMN: Contact Form -->
  <div class="bg-white dark:bg-neutral-800 p-6 md:p-8 rounded-2xl shadow-sm border border-neutral-100 dark:border-neutral-700">
    <h2 class="text-2xl font-bold mb-6">Send a Message</h2>
    
    <!-- 
      Formspree Contact Form 
      1. 登录 https://formspree.io/ 注册
      2. 创建一个新 Form
      3. 将下面的 "YOUR_FORM_ID" 替换为你获得的 ID (例如: xdoqplkz)
    -->
    <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST" class="space-y-4">
      
      <!-- Name -->
      <div>
        <label for="name" class="block text-sm font-medium text-neutral-700 dark:text-neutral-300 mb-1">Name</label>
        <input type="text" name="name" id="name" required
          class="w-full px-4 py-2 rounded-lg bg-neutral-50 dark:bg-neutral-900 border border-neutral-200 dark:border-neutral-700 focus:ring-2 focus:ring-primary-500 focus:border-transparent outline-none transition-all">
      </div>

      <!-- Email -->
      <div>
        <label for="email" class="block text-sm font-medium text-neutral-700 dark:text-neutral-300 mb-1">Email</label>
        <input type="email" name="email" id="email" required
          class="w-full px-4 py-2 rounded-lg bg-neutral-50 dark:bg-neutral-900 border border-neutral-200 dark:border-neutral-700 focus:ring-2 focus:ring-primary-500 focus:border-transparent outline-none transition-all">
      </div>

      <!-- Subject -->
      <div>
        <label for="subject" class="block text-sm font-medium text-neutral-700 dark:text-neutral-300 mb-1">Subject</label>
        <select name="subject" id="subject"
          class="w-full px-4 py-2 rounded-lg bg-neutral-50 dark:bg-neutral-900 border border-neutral-200 dark:border-neutral-700 focus:ring-2 focus:ring-primary-500 focus:border-transparent outline-none transition-all">
          <option value="General">👋 Just saying hi</option>
          <option value="Project">💼 Project collaboration</option>
          <option value="Bug">🐛 Bug report</option>
          <option value="Other">Other</option>
        </select>
      </div>

      <!-- Message -->
      <div>
        <label for="message" class="block text-sm font-medium text-neutral-700 dark:text-neutral-300 mb-1">Message</label>
        <textarea name="message" id="message" rows="5" required
          class="w-full px-4 py-2 rounded-lg bg-neutral-50 dark:bg-neutral-900 border border-neutral-200 dark:border-neutral-700 focus:ring-2 focus:ring-primary-500 focus:border-transparent outline-none transition-all resize-none"></textarea>
      </div>

      <!-- Submit Button -->
      <button type="submit" 
        class="w-full py-3 px-4 bg-primary-600 hover:bg-primary-700 text-white font-medium rounded-lg shadow-md hover:shadow-lg transition-all transform active:scale-95 flex justify-center items-center gap-2">
        <span>Send Message</span>
        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="22" x2="11" y1="2" y2="13"/><polygon points="22 2 15 22 11 13 2 9"/></svg>
      </button>

    </form>
  </div>
</div>

---

<!-- Optional: Schedule a Call Section -->
<div class="mt-16 text-center">
  <h2 class="text-2xl font-bold mb-4">Prefer a video call?</h2>
  <p class="text-neutral-500 dark:text-neutral-400 mb-6 max-w-lg mx-auto">
    如果你的事情比较复杂，或者你更喜欢面对面交流，可以直接预约我的时间。
  </p>
  
  <!-- Cal.com or Calendly Link -->
  <a href="https://calendly.com/" target="_blank" 
     class="inline-flex items-center gap-2 px-6 py-3 rounded-full bg-neutral-900 dark:bg-white text-white dark:text-black font-semibold hover:opacity-80 transition-opacity">
     <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect width="18" height="18" x="3" y="4" rx="2" ry="2"/><line x1="16" x2="16" y1="2" y2="6"/><line x1="8" x2="8" y1="2" y2="6"/><line x1="3" x2="21" y1="10" y2="10"/></svg>
     <span>Book a 15min Call</span>
  </a>
</div>

<script>
  function copyEmail(element) {
    const email = document.getElementById('email-text').innerText;
    navigator.clipboard.writeText(email).then(() => {
      // Visual feedback
      const originalBg = element.firstElementChild.className;
      element.firstElementChild.classList.add('bg-green-50', 'dark:bg-green-900', 'border-green-200');
      
      const codeElem = document.getElementById('email-text');
      const originalText = codeElem.innerText;
      codeElem.innerText = "Copied! ✅";
      
      setTimeout(() => {
        element.firstElementChild.className = originalBg; // Reset classes could be cleaner but this works for demo
        element.firstElementChild.classList.remove('bg-green-50', 'dark:bg-green-900', 'border-green-200');
        codeElem.innerText = originalText;
      }, 2000);
    });
  }
</script>