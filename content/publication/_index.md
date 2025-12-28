---
title: "Publications"
description: "Selected peer-reviewed journals and conference proceedings."
layout: "single"
showTaxonomies: false
showTableOfContents: false
---

<!-- 引入简单的 Alpine.js 逻辑用于筛选 -->
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

    <!-- 介绍部分 -->
    <div class="mb-10">
        <p class="text-lg text-neutral-600 dark:text-neutral-400">
            我的研究主要集中在计算机视觉和深度学习。以下是发表的论文列表。
            <br> (注：* 表示共同一作，下划线表示通讯作者)
        </p>
    </div>

    <!-- 筛选器布局 -->
    <div class="bg-neutral-50 dark:bg-neutral-800 p-6 rounded-xl mb-12 border border-neutral-200 dark:border-neutral-700">
        <div class="flex flex-wrap gap-4 items-center">
            
            <!-- 年份筛选 -->
            <div class="flex flex-col">
                <span class="text-xs font-bold uppercase mb-1 opacity-60">Year</span>
                <select x-model="filterYear" class="bg-white dark:bg-neutral-900 border-neutral-300 dark:border-neutral-700 rounded text-sm p-1">
                    <option value="All">All Years</option>
                    <option value="2024">2024</option>
                    <option value="2023">2023</option>
                    <option value="2022">2022</option>
                </select>
            </div>

            <!-- 标签筛选 -->
            <div class="flex flex-col">
                <span class="text-xs font-bold uppercase mb-1 opacity-60">Category</span>
                <select x-model="filterTag" class="bg-white dark:bg-neutral-900 border-neutral-300 dark:border-neutral-700 rounded text-sm p-1">
                    <option value="All">All Types</option>
                    <option value="Conference">Conference</option>
                    <option value="Journal">Journal</option>
                    <option value="Preprint">Preprint</option>
                </select>
            </div>

            <!-- 期刊/会议筛选 -->
            <div class="flex flex-col">
                <span class="text-xs font-bold uppercase mb-1 opacity-60">Venue</span>
                <select x-model="filterJournal" class="bg-white dark:bg-neutral-900 border-neutral-300 dark:border-neutral-700 rounded text-sm p-1">
                    <option value="All">All Venues</option>
                    <option value="CVPR">CVPR</option>
                    <option value="Nature">Nature</option>
                    <option value="IEEE TNNLS">IEEE TNNLS</option>
                </select>
            </div>

            <!-- 第一作者开关 -->
            <div class="flex items-center mt-5 ml-2">
                <input type="checkbox" x-model="filterFirstAuthor" id="firstAuthor" class="mr-2">
                <label for="firstAuthor" class="text-sm font-medium cursor-pointer">First Author Only</label>
            </div>

            <!-- 重置按钮 -->
            <button @click="filterYear='All'; filterTag='All'; filterJournal='All'; filterFirstAuthor=false" 
                    class="mt-5 ml-auto text-xs underline opacity-60 hover:opacity-100">
                Reset Filters
            </button>
        </div>
    </div>

    <!-- 论文列表 -->
    <div class="space-y-8">

        <!-- 论文项目 1 -->
        <div x-show="showItem('2024', ['Conference', 'Computer Vision'], 'CVPR', 'true')" 
             class="group relative flex flex-col md:flex-row gap-6 p-4 rounded-2xl transition-all hover:bg-neutral-100 dark:hover:bg-neutral-800 border border-transparent hover:border-neutral-200 dark:hover:border-neutral-700">
            
            <div class="w-full md:w-1/4 shrink-0">
                <img src="/images/pub-teaser-1.png" alt="Paper Teaser" class="rounded-lg shadow-sm border border-neutral-200 dark:border-neutral-700 w-full h-auto object-cover">
            </div>

            <div class="flex-grow">
                <div class="flex items-center gap-2 mb-2">
                    <span class="px-2 py-0.5 text-[10px] font-bold tracking-wider uppercase bg-primary-100 text-primary-700 dark:bg-primary-900 dark:text-primary-200 rounded">CVPR 2024</span>
                    <span class="px-2 py-0.5 text-[10px] font-bold tracking-wider uppercase bg-neutral-200 dark:bg-neutral-700 rounded">Oral</span>
                </div>
                
                <h3 class="text-xl font-bold mb-2 group-hover:text-primary-600 transition-colors">
                    Innovative Deep Learning Architecture for Real-time Scene Understanding
                </h3>
                
                <div class="text-sm mb-3">
                    <strong>Your Name*</strong>, Jane Doe*, John Smith, <span class="underline">Advisor Name</span>
                </div>

                <div class="flex flex-wrap gap-2 mb-4">
                    {{< badge >}}Computer Vision{{< /badge >}}
                    {{< badge >}}Scene Parsing{{< /badge >}}
                </div>

                <div class="flex gap-4 text-sm font-medium">
                    <a href="#" class="flex items-center gap-1 text-primary-600 hover:underline">{{< icon "paper" >}} Paper</a>
                    <a href="#" class="flex items-center gap-1 text-primary-600 hover:underline">{{< icon "github" >}} Code</a>
                    <a href="#" class="flex items-center gap-1 text-primary-600 hover:underline">{{< icon "quote" >}} BibTeX</a>
                    <a href="#" class="flex items-center gap-1 text-primary-600 hover:underline">{{< icon "video" >}} Video</a>
                </div>
            </div>
        </div>

        <!-- 论文项目 2 -->
        <div x-show="showItem('2023', ['Journal', 'Deep Learning'], 'IEEE TNNLS', 'false')" 
             class="group relative flex flex-col md:flex-row gap-6 p-4 rounded-2xl transition-all hover:bg-neutral-100 dark:hover:bg-neutral-800 border border-transparent hover:border-neutral-200 dark:hover:border-neutral-700">
            
            <div class="w-full md:w-1/4 shrink-0">
                <img src="/images/pub-teaser-2.png" alt="Paper Teaser" class="rounded-lg shadow-sm border border-neutral-200 dark:border-neutral-700 w-full h-auto object-cover">
            </div>

            <div class="flex-grow">
                <div class="flex items-center gap-2 mb-2">
                    <span class="px-2 py-0.5 text-[10px] font-bold tracking-wider uppercase bg-secondary-100 text-secondary-700 dark:bg-secondary-900 dark:text-secondary-200 rounded">IEEE TNNLS 2023</span>
                </div>
                
                <h3 class="text-xl font-bold mb-2 group-hover:text-primary-600 transition-colors">
                    A Comprehensive Survey on Robust Neural Networks
                </h3>
                
                <div class="text-sm mb-3">
                    Jane Doe, <strong>Your Name</strong>, John Smith
                </div>

                <div class="flex flex-wrap gap-2 mb-4">
                    {{< badge >}}Deep Learning{{< /badge >}}
                    {{< badge >}}Survey{{< /badge >}}
                </div>

                <div class="flex gap-4 text-sm font-medium">
                    <a href="#" class="flex items-center gap-1 text-primary-600 hover:underline">{{< icon "paper" >}} PDF</a>
                    <a href="#" class="flex items-center gap-1 text-primary-600 hover:underline">{{< icon "quote" >}} BibTeX</a>
                </div>
            </div>
        </div>

        <!-- 更多论文... 复制上方 div 并修改参数 -->

    </div>

    <!-- 无搜索结果提示 -->
    <div x-cloak x-show="!document.querySelector('.space-y-8').innerText.trim()" class="text-center py-20">
        <p class="text-neutral-500">没有找到符合条件的论文。</p>
    </div>

</div>