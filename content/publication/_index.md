---
title: "Publications"
description: "Selected peer-reviewed journals and conference proceedings."
layout: "single"
---

<!-- 引入 Font Awesome 网络库 -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css">

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

    <!-- 1. 筛选面板 -->
    <div class="bg-neutral-50 dark:bg-neutral-800 p-6 rounded-2xl mb-12 border border-neutral-200 dark:border-neutral-700 shadow-sm">
        <div class="grid grid-cols-1 md:grid-cols-4 gap-6 items-end">
            
            <!-- 年份 -->
            <div class="flex flex-col">
                <label class="text-xs font-bold uppercase mb-2 opacity-60"><i class="fa-solid fa-calendar-days mr-1"></i> Year</label>
                <select x-model="filterYear" class="bg-white dark:bg-neutral-900 border-neutral-300 dark:border-neutral-700 rounded-lg text-sm p-2 focus:ring-primary-500">
                    <option value="All">All Years</option>
                    <option value="2024">2024</option>
                    <option value="2023">2023</option>
                </select>
            </div>

            <!-- 类别 -->
            <div class="flex flex-col">
                <label class="text-xs font-bold uppercase mb-2 opacity-60"><i class="fa-solid fa-tag mr-1"></i> Category</label>
                <select x-model="filterTag" class="bg-white dark:bg-neutral-900 border-neutral-300 dark:border-neutral-700 rounded-lg text-sm p-2">
                    <option value="All">All Types</option>
                    <option value="Conference">Conference</option>
                    <option value="Journal">Journal</option>
                </select>
            </div>

            <!-- 期刊 -->
            <div class="flex flex-col">
                <label class="text-xs font-bold uppercase mb-2 opacity-60"><i class="fa-solid fa-building-columns mr-1"></i> Venue</label>
                <select x-model="filterJournal" class="bg-white dark:bg-neutral-900 border-neutral-300 dark:border-neutral-700 rounded-lg text-sm p-2">
                    <option value="All">All Venues</option>
                    <option value="CVPR">CVPR</option>
                    <option value="Nature">Nature</option>
                </select>
            </div>

            <!-- 第一作者 -->
            <div class="flex items-center pb-2 h-10">
                <label class="relative inline-flex items-center cursor-pointer">
                    <input type="checkbox" x-model="filterFirstAuthor" class="sr-only peer">
                    <div class="w-11 h-6 bg-neutral-200 peer-focus:outline-none rounded-full peer dark:bg-neutral-700 peer-checked:after:translate-x-full peer-checked:after:border-white after:content-[''] after:absolute after:top-[2px] after:left-[2px] after:bg-white after:border-gray-300 after:border after:rounded-full after:h-5 after:w-5 after:transition-all peer-checked:bg-primary-500"></div>
                    <span class="ml-3 text-sm font-medium">First Author</span>
                </label>
            </div>
        </div>
        <!-- 重置 -->
        <div class="mt-4 flex justify-end">
            <button @click="filterYear='All'; filterTag='All'; filterJournal='All'; filterFirstAuthor=false" class="text-xs text-primary-500 hover:underline">
                <i class="fa-solid fa-rotate-left mr-1"></i> Reset Filters
            </button>
        </div>
    </div>

    <!-- 2. 论文列表 -->
    <div class="space-y-10">

        <!-- 论文条目 1 -->
        <div x-show="showItem('2024', ['Conference'], 'CVPR', 'true')" 
             class="group flex flex-col md:flex-row gap-8 transition-opacity duration-300">
            
            <!-- 缩略图 -->
            <div class="w-full md:w-56 shrink-0">
                <div class="relative overflow-hidden rounded-lg border border-neutral-200 dark:border-neutral-700 shadow-sm transition-transform group-hover:scale-[1.02]">
                    <img src="/images/your-paper-image.png" alt="Teaser" class="w-full h-32 object-cover">
                </div>
            </div>

            <!-- 内容 -->
            <div class="flex-grow">
                <div class="flex items-center gap-2 mb-3">
                    <span class="bg-primary-100 dark:bg-primary-900 text-primary-800 dark:text-primary-200 text-[10px] font-black px-2 py-0.5 rounded uppercase tracking-widest">CVPR 2024</span>
                    <span class="bg-neutral-100 dark:bg-neutral-700 text-neutral-600 dark:text-neutral-300 text-[10px] font-bold px-2 py-0.5 rounded uppercase">Oral</span>
                </div>
                
                <h3 class="text-xl font-extrabold mb-2 group-hover:text-primary-500 transition-colors">
                    Innovative Research Title for Machine Learning Applications
                </h3>
                
                <div class="text-neutral-600 dark:text-neutral-400 text-sm mb-4">
                    <b class="text-neutral-900 dark:text-neutral-100 decoration-primary-500 underline decoration-2">Your Name*</b>, Co-author, and Advisor
                </div>

                <!-- 链接按钮 -->
                <div class="flex flex-wrap gap-4 items-center">
                    <a href="#" class="inline-flex items-center text-xs font-bold text-neutral-500 hover:text-primary-500 transition-colors">
                        <i class="fa-solid fa-file-pdf mr-1.5 text-base"></i> PAPER
                    </a>
                    <a href="#" class="inline-flex items-center text-xs font-bold text-neutral-500 hover:text-primary-500 transition-colors">
                        <i class="fa-brands fa-github mr-1.5 text-base"></i> CODE
                    </a>
                    <a href="#" class="inline-flex items-center text-xs font-bold text-neutral-500 hover:text-primary-500 transition-colors">
                        <i class="fa-solid fa-quote-left mr-1.5 text-base"></i> BIBTEX
                    </a>
                    <a href="#" class="inline-flex items-center text-xs font-bold text-neutral-500 hover:text-primary-500 transition-colors">
                        <i class="fa-solid fa-video mr-1.5 text-base"></i> VIDEO
                    </a>
                </div>
            </div>
        </div>

        <!-- 论文条目 2 -->
        <div x-show="showItem('2023', ['Journal'], 'Nature', 'false')" 
             class="group flex flex-col md:flex-row gap-8 transition-opacity duration-300">
            <div class="w-full md:w-56 shrink-0">
                <div class="relative overflow-hidden rounded-lg border border-neutral-200 dark:border-neutral-700 shadow-sm transition-transform group-hover:scale-[1.02]">
                    <img src="/images/another-paper.png" alt="Teaser" class="w-full h-32 object-cover">
                </div>
            </div>
            <div class="flex-grow">
                <div class="flex items-center gap-2 mb-3">
                    <span class="bg-secondary-100 dark:bg-secondary-900 text-secondary-800 dark:text-secondary-200 text-[10px] font-black px-2 py-0.5 rounded uppercase tracking-widest">Nature 2023</span>
                </div>
                <h3 class="text-xl font-extrabold mb-2 group-hover:text-primary-500 transition-colors">
                    A Major Scientific Breakthrough in Neutral Networks
                </h3>
                <div class="text-neutral-600 dark:text-neutral-400 text-sm mb-4">
                    First Author, <b class="text-neutral-900 dark:text-neutral-100 underline decoration-primary-500 decoration-2">Your Name</b>, and Senior Author
                </div>
                <div class="flex flex-wrap gap-4 items-center">
                    <a href="#" class="inline-flex items-center text-xs font-bold text-neutral-500 hover:text-primary-500 transition-colors">
                        <i class="fa-solid fa-file-lines mr-1.5 text-base"></i> PDF
                    </a>
                    <a href="#" class="inline-flex items-center text-xs font-bold text-neutral-500 hover:text-primary-500 transition-colors">
                        <i class="fa-solid fa-share-nodes mr-1.5 text-base"></i> PROJECT
                    </a>
                </div>
            </div>
        </div>

    </div>

    <!-- 3. 无结果提示 -->
    <div x-show="!$el.parentElement.querySelectorAll('.group[style*=\'display: none\']').length === $el.parentElement.querySelectorAll('.group').length" class="hidden">
        <!-- 这里的逻辑稍微复杂，Alpine 简单处理可直接显示： -->
    </div>

</div>