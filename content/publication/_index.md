---
title: "Publications"
description: "Selected peer-reviewed journals and conference proceedings."
layout: "single"
---

<!-- 1. 引入 Font Awesome 确保图标正常 -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css">

<!-- 2. Alpine.js 容器开始 -->
<div x-data="{ 
    filterYear: 'All', 
    filterTag: 'All', 
    filterJournal: 'All',
    filterFirstAuthor: false,
    showItem(year, tags, journal, isFirst) {
        const matchYear = (this.filterYear === 'All' || this.filterYear === year);
        const matchTag = (this.filterTag === 'All' || tags.includes(this.filterTag));
        const matchJournal = (this.filterJournal === 'All' || journal === this.filterJournal);
        const matchFirst = (!this.filterFirstAuthor || isFirst === 'true');
        return matchYear && matchTag && matchJournal && matchFirst;
    }
}">

<!-- 筛选面板 -->
<div class="bg-neutral-50 dark:bg-neutral-800 p-6 rounded-2xl mb-12 border border-neutral-200 dark:border-neutral-700 shadow-sm">
    <div class="grid grid-cols-1 md:grid-cols-4 gap-6 items-end">
        
        <!-- 年份 -->
        <div class="flex flex-col text-left">
            <label class="text-xs font-bold uppercase mb-2 opacity-60"><i class="fa-solid fa-calendar-days mr-1"></i> Year</label>
            <select x-model="filterYear" class="w-full bg-white dark:bg-neutral-900 border-neutral-300 dark:border-neutral-700 rounded-lg text-sm p-2">
                <option value="All">All Years</option>
                <option value="2024">2024</option>
                <option value="2023">2023</option>
            </select>
        </div>

        <!-- 类别 -->
        <div class="flex flex-col text-left">
            <label class="text-xs font-bold uppercase mb-2 opacity-60"><i class="fa-solid fa-tag mr-1"></i> Category</label>
            <select x-model="filterTag" class="w-full bg-white dark:bg-neutral-900 border-neutral-300 dark:border-neutral-700 rounded-lg text-sm p-2">
                <option value="All">All Types</option>
                <option value="Conference">Conference</option>
                <option value="Journal">Journal</option>
            </select>
        </div>

        <!-- 期刊 -->
        <div class="flex flex-col text-left">
            <label class="text-xs font-bold uppercase mb-2 opacity-60"><i class="fa-solid fa-building-columns mr-1"></i> Venue</label>
            <select x-model="filterJournal" class="w-full bg-white dark:bg-neutral-900 border-neutral-300 dark:border-neutral-700 rounded-lg text-sm p-2">
                <option value="All">All Venues</option>
                <option value="CVPR">CVPR</option>
                <option value="Nature">Nature</option>
            </select>
        </div>

        <!-- 第一作者开关 -->
        <div class="flex items-center pb-2 h-10">
            <label class="relative inline-flex items-center cursor-pointer">
                <input type="checkbox" x-model="filterFirstAuthor" class="sr-only peer">
                <div class="w-11 h-6 bg-neutral-200 rounded-full peer dark:bg-neutral-700 peer-checked:after:translate-x-full peer-checked:bg-primary-500 after:content-[''] after:absolute after:top-[2px] after:left-[2px] after:bg-white after:rounded-full after:h-5 after:w-5 after:transition-all"></div>
                <span class="ml-3 text-sm font-medium">1st Author Only</span>
            </label>
        </div>
    </div>
    
    <div class="mt-4 flex justify-end">
        <button @click="filterYear='All'; filterTag='All'; filterJournal='All'; filterFirstAuthor=false" class="text-xs text-primary-500 hover:underline">
            <i class="fa-solid fa-rotate-left mr-1"></i> Reset Filters
        </button>
    </div>
</div>

<!-- 论文列表 -->
<div class="space-y-10">

    <!-- 论文条目 1 -->
    <div x-show="showItem('2024', ['Conference'], 'CVPR', 'true')" 
         class="group flex flex-col md:flex-row gap-8 transition-all duration-300 border-b border-neutral-100 dark:border-neutral-800 pb-8">
        
        <div class="w-full md:w-56 shrink-0">
            <div class="relative overflow-hidden rounded-lg border border-neutral-200 dark:border-neutral-700 shadow-sm transition-transform group-hover:scale-[1.02]">
                <img src="/images/paper1.png" alt="Teaser" class="w-full h-32 object-cover bg-neutral-100">
            </div>
        </div>

        <div class="flex-grow">
            <div class="flex items-center gap-2 mb-3">
                <span class="bg-primary-100 dark:bg-primary-900 text-primary-800 dark:text-primary-200 text-[10px] font-black px-2 py-0.5 rounded uppercase tracking-widest">CVPR 2024</span>
            </div>
            <h3 class="text-xl font-extrabold mb-2 group-hover:text-primary-500 transition-colors">
                Towards Scalable Visual Representation Learning
            </h3>
            <div class="text-neutral-600 dark:text-neutral-400 text-sm mb-4">
                <b class="text-neutral-900 dark:text-neutral-100 underline decoration-primary-500 decoration-2">Your Name*</b>, Jane Smith, and John Doe
            </div>
            <div class="flex flex-wrap gap-4 items-center">
                <a href="#" class="inline-flex items-center text-xs font-bold text-neutral-500 hover:text-primary-500 transition-colors">
                    <i class="fa-solid fa-file-pdf mr-1.5 text-base"></i> PAPER
                </a>
                <a href="#" class="inline-flex items-center text-xs font-bold text-neutral-500 hover:text-primary-500 transition-colors">
                    <i class="fa-brands fa-github mr-1.5 text-base"></i> CODE
                </a>
            </div>
        </div>
    </div>

    <!-- 论文条目 2 -->
    <div x-show="showItem('2023', ['Journal'], 'Nature', 'false')" 
         class="group flex flex-col md:flex-row gap-8 transition-all duration-300 border-b border-neutral-100 dark:border-neutral-800 pb-8">
        <div class="w-full md:w-56 shrink-0">
            <div class="relative overflow-hidden rounded-lg border border-neutral-200 dark:border-neutral-700 shadow-sm transition-transform group-hover:scale-[1.02]">
                <img src="/images/paper2.png" alt="Teaser" class="w-full h-32 object-cover bg-neutral-100">
            </div>
        </div>
        <div class="flex-grow">
            <div class="flex items-center gap-2 mb-3">
                <span class="bg-secondary-100 dark:bg-secondary-900 text-secondary-800 dark:text-secondary-200 text-[10px] font-black px-2 py-0.5 rounded uppercase tracking-widest">Nature 2023</span>
            </div>
            <h3 class="text-xl font-extrabold mb-2 group-hover:text-primary-500 transition-colors">
                Advancing Science with High-Performance Computing
            </h3>
            <div class="text-neutral-600 dark:text-neutral-400 text-sm mb-4">
                Jane Smith, <b class="text-neutral-900 dark:text-neutral-100 underline decoration-primary-500 decoration-2">Your Name</b>, and John Doe
            </div>
            <div class="flex flex-wrap gap-4 items-center">
                <a href="#" class="inline-flex items-center text-xs font-bold text-neutral-500 hover:text-primary-500 transition-colors">
                    <i class="fa-solid fa-file-lines mr-1.5 text-base"></i> PDF
                </a>
            </div>
        </div>
    </div>

</div>

<!-- 无搜索结果提示 -->
<div x-show="false" class="py-20 text-center text-neutral-500">
    No publications found matching the selected filters.
</div>

</div>