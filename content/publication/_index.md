---
title: "Publications"
description: "Selected peer-reviewed journals and conference proceedings."
layout: "docs"
showTableOfContents: true
---

<!-- 引入依赖库 -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css">

<div x-data="{ 
    activeYear: 'All', 
    activeTag: 'All', 
    firstAuthorOnly: false,
    // 核心筛选逻辑
    shouldShow(year, tags, isFirst) {
        const yearMatch = this.activeYear === 'All' || this.activeYear === year;
        const tagMatch = this.activeTag === 'All' || tags.includes(this.activeTag);
        const authorMatch = !this.firstAuthorOnly || isFirst === 'true';
        return yearMatch && tagMatch && authorMatch;
    }
}">

<!-- 1. 成果概览统计 (Stats) -->
<div class="grid grid-cols-2 md:grid-cols-4 gap-4 mb-10 text-center">
    <div class="p-4 bg-neutral-50 dark:bg-neutral-800 rounded-2xl border border-neutral-200 dark:border-neutral-700">
        <div class="text-2xl font-bold text-primary-600">15</div>
        <div class="text-xs uppercase tracking-widest opacity-60">Total Papers</div>
    </div>
    <div class="p-4 bg-neutral-50 dark:bg-neutral-800 rounded-2xl border border-neutral-200 dark:border-neutral-700">
        <div class="text-2xl font-bold text-primary-600">10</div>
        <div class="text-xs uppercase tracking-widest opacity-60">Journals</div>
    </div>
    <div class="p-4 bg-neutral-50 dark:bg-neutral-800 rounded-2xl border border-neutral-200 dark:border-neutral-700">
        <div class="text-2xl font-bold text-primary-600">5</div>
        <div class="text-xs uppercase tracking-widest opacity-60">Conferences</div>
    </div>
    <div class="p-4 bg-neutral-50 dark:bg-neutral-800 rounded-2xl border border-neutral-200 dark:border-neutral-700">
        <div class="text-2xl font-bold text-primary-600">3</div>
        <div class="text-xs uppercase tracking-widest opacity-60">1st Author</div>
    </div>
</div>

<!-- 2. 动态筛选交互区 -->
<div class="sticky top-20 z-10 bg-white/80 dark:bg-neutral-900/80 backdrop-blur-md py-4 mb-8 border-b border-neutral-200 dark:border-neutral-800">
    <div class="flex flex-col gap-4">
        <!-- 年份筛选 -->
        <div class="flex items-center gap-3 flex-wrap">
            <span class="text-xs font-bold uppercase opacity-50"><i class="fa-solid fa-calendar mr-1"></i> Year:</span>
            <template x-for="year in ['All', '2024', '2023']">
                <button @click="activeYear = year" 
                    :class="activeYear === year ? 'bg-primary-500 text-white' : 'bg-neutral-100 dark:bg-neutral-800 hover:bg-neutral-200'"
                    class="px-3 py-1 rounded-full text-xs font-medium transition-all" x-text="year"></button>
            </template>
        </div>
        <!-- 领域筛选 -->
        <div class="flex items-center gap-3 flex-wrap">
            <span class="text-xs font-bold uppercase opacity-50"><i class="fa-solid fa-flask mr-1"></i> Topic:</span>
            <template x-for="tag in ['All', 'AI/ML', 'Computer Vision', 'Systems']">
                <button @click="activeTag = tag" 
                    :class="activeTag === tag ? 'bg-secondary-500 text-white' : 'bg-neutral-100 dark:bg-neutral-800 hover:bg-neutral-200'"
                    class="px-3 py-1 rounded-full text-xs font-medium transition-all" x-text="tag"></button>
            </template>
            <!-- 第一作者开关 -->
            <label class="ml-auto inline-flex items-center cursor-pointer">
                <input type="checkbox" x-model="firstAuthorOnly" class="sr-only peer">
                <div class="w-9 h-5 bg-neutral-200 peer-focus:outline-none rounded-full peer dark:bg-neutral-700 peer-checked:after:translate-x-full peer-checked:bg-primary-500 after:content-[''] after:absolute after:top-[2px] after:left-[2px] after:bg-white after:rounded-full after:h-4 after:w-4 after:transition-all"></div>
                <span class="ml-2 text-xs font-bold uppercase opacity-70">1st Author Only</span>
            </label>
        </div>
    </div>
</div>

<!-- 3. 正文内容 - 使用 Markdown 标题以生成右侧 TOC -->

## Journal Articles

<div class="grid grid-cols-1 gap-6">

    <!-- 论文卡片 1 -->
    <div x-show="shouldShow('2024', ['AI/ML'], 'true')" 
         class="group p-6 bg-white dark:bg-neutral-900 border border-neutral-200 dark:border-neutral-800 rounded-2xl shadow-sm hover:shadow-md hover:border-primary-500/50 transition-all duration-300">
        <div class="flex flex-wrap items-center gap-2 mb-3">
            <span class="px-2 py-0.5 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-200 text-[10px] font-bold rounded">2024</span>
            <span class="px-2 py-0.5 bg-neutral-100 dark:bg-neutral-800 text-neutral-600 dark:text-neutral-400 text-[10px] font-bold rounded uppercase">Journal</span>
        </div>
        <h3 class="text-lg font-bold mb-2 group-hover:text-primary-600 transition-colors">Towards Scalable Visual Representation Learning with Masked Generative Pretraining</h3>
        <p class="text-sm text-neutral-600 dark:text-neutral-400 mb-4 leading-relaxed">
            <span class="font-bold text-neutral-900 dark:text-neutral-100 underline decoration-primary-500 decoration-2 text-underline-offset-4">Your Name*</span>, Jane Smith, John Doe, Robert Brown
            <br>
            <span class="italic">IEEE Transactions on Pattern Analysis and Machine Intelligence (TPAMI)</span>
        </p>
        <div class="flex flex-wrap gap-3 mt-4">
            <a href="#" class="inline-flex items-center text-xs font-bold text-primary-600 hover:text-primary-700"><i class="fa-solid fa-file-pdf mr-1.5"></i> PDF</a>
            <a href="#" class="inline-flex items-center text-xs font-bold text-neutral-500 hover:text-primary-600"><i class="fa-brands fa-github mr-1.5"></i> CODE</a>
            <a href="#" class="inline-flex items-center text-xs font-bold text-neutral-500 hover:text-primary-600"><i class="fa-solid fa-quote-right mr-1.5"></i> BIBTEX</a>
        </div>
    </div>

    <!-- 论文卡片 2 -->
    <div x-show="shouldShow('2023', ['Systems'], 'true')" 
         class="group p-6 bg-white dark:bg-neutral-900 border border-neutral-200 dark:border-neutral-800 rounded-2xl shadow-sm hover:shadow-md hover:border-primary-500/50 transition-all duration-300">
        <div class="flex flex-wrap items-center gap-2 mb-3">
            <span class="px-2 py-0.5 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-200 text-[10px] font-bold rounded">2023</span>
            <span class="px-2 py-0.5 bg-neutral-100 dark:bg-neutral-800 text-neutral-600 dark:text-neutral-400 text-[10px] font-bold rounded uppercase">Journal</span>
        </div>
        <h3 class="text-lg font-bold mb-2 group-hover:text-primary-600 transition-colors">Efficient Federated Learning for Edge Computing</h3>
        <p class="text-sm text-neutral-600 dark:text-neutral-400 mb-4 leading-relaxed">
            <span class="font-bold text-neutral-900 dark:text-neutral-100 underline decoration-primary-500 decoration-2 text-underline-offset-4">Your Name*</span>, Alice Johnson, Bob Wilson
            <br>
            <span class="italic">ACM Transactions on Intelligent Systems and Technology (TIST)</span>
        </p>
        <div class="flex flex-wrap gap-3 mt-4">
            <a href="#" class="inline-flex items-center text-xs font-bold text-primary-600 hover:text-primary-700"><i class="fa-solid fa-link mr-1.5"></i> DOI</a>
            <a href="#" class="inline-flex items-center text-xs font-bold text-neutral-500 hover:text-primary-600"><i class="fa-brands fa-github mr-1.5"></i> CODE</a>
        </div>
    </div>

</div>

## Conference Proceedings

<div class="grid grid-cols-1 gap-6">

    <!-- 论文卡片 3 -->
    <div x-show="shouldShow('2024', ['Computer Vision'], 'true')" 
         class="group p-6 bg-white dark:bg-neutral-900 border border-neutral-200 dark:border-neutral-800 rounded-2xl shadow-sm hover:shadow-md hover:border-primary-500/50 transition-all duration-300">
        <div class="flex flex-wrap items-center gap-2 mb-3">
            <span class="px-2 py-0.5 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-200 text-[10px] font-bold rounded">2024</span>
            <span class="px-2 py-0.5 bg-purple-100 dark:bg-purple-900 text-purple-700 dark:text-purple-200 text-[10px] font-bold rounded uppercase">Conference</span>
        </div>
        <h3 class="text-lg font-bold mb-2 group-hover:text-primary-600 transition-colors">Dynamic Neural Radiance Fields for Real-time View Synthesis</h3>
        <p class="text-sm text-neutral-600 dark:text-neutral-400 mb-4 leading-relaxed">
            <span class="font-bold text-neutral-900 dark:text-neutral-100 underline decoration-primary-500 decoration-2 text-underline-offset-4">Your Name*</span>, Carol Davis, Michael Lee
            <br>
            <span class="italic">CVPR 2024 (Oral)</span>
        </p>
        <div class="flex flex-wrap gap-3 mt-4">
            <a href="#" class="inline-flex items-center text-xs font-bold text-primary-600 hover:text-primary-700"><i class="fa-solid fa-file-pdf mr-1.5"></i> PDF</a>
            <a href="#" class="inline-flex items-center text-xs font-bold text-neutral-500 hover:text-primary-600"><i class="fa-solid fa-globe mr-1.5"></i> PROJECT</a>
        </div>
    </div>

</div>

## Preprints

<div class="grid grid-cols-1 gap-6">
    <!-- 更多内容... -->
</div>

<!-- 无结果提示 -->
<div x-show="activeYear !== 'All' && activeTag !== 'All' && $el.parentElement.querySelectorAll('.group[style*=\'display: none\']').length === $el.parentElement.querySelectorAll('.group').length" 
     class="py-20 text-center opacity-50 font-medium">
    No publications matching the selected filters.
</div>

</div>

<hr class="my-12 opacity-10">

<div class="flex flex-col md:flex-row justify-between items-center gap-4 text-sm opacity-60 italic">
    <div>* indicates corresponding author / equal contribution.</div>
    <div class="flex gap-4">
        <a href="#" class="hover:text-primary-500 transition-colors">Google Scholar</a>
        <a href="#" class="hover:text-primary-500 transition-colors">ORCID</a>
        <a href="#" class="hover:text-primary-500 transition-colors">GitHub</a>
    </div>
</div>