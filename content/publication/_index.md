---
title: "Publications"
description: "Selected peer-reviewed journals and conference proceedings."
layout: "simple"
fullWidth: true
---

<!-- 引入 FontAwesome 图标库 (如果你的主题未包含) -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<style>
/* 核心变量定义 - 方便统一调整 */
:root {
    --primary-color: #2563eb;       /* 学术蓝 */
    --primary-hover: #1d4ed8;
    --bg-card: #ffffff;
    --border-color: #e5e7eb;
    --text-main: #111827;
    --text-muted: #6b7280;
    --tag-bg: #f3f4f6;
    --tag-text: #374151;
    --award-color: #d97706;         /* 奖项金 */
    --transition-speed: 0.2s;
}

/* 暗色模式适配 */
.dark {
    --bg-card: #1f2937;
    --border-color: #374151;
    --text-main: #f3f4f6;
    --text-muted: #9ca3af;
    --tag-bg: #374151;
    --tag-text: #d1d5db;
}

/* 工具栏区域 (统计 + 搜索 + 筛选) */
.pub-toolbar {
    margin-bottom: 2rem;
}

/* 统计卡片 - 更加紧凑 */
.stats-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 1rem;
    background: var(--tag-bg);
    padding: 1.5rem;
    border-radius: 12px;
    margin-bottom: 2rem;
    text-align: center;
}

.stat-item h4 {
    font-size: 2rem;
    font-weight: 700;
    color: var(--primary-color);
    margin: 0;
    line-height: 1;
}

.stat-item p {
    font-size: 0.85rem;
    color: var(--text-muted);
    margin: 0.5rem 0 0 0;
    font-weight: 500;
}

/* 搜索框 */
.search-wrapper {
    position: relative;
    margin-bottom: 1.5rem;
}

.search-input {
    width: 100%;
    padding: 12px 20px 12px 45px;
    border: 1px solid var(--border-color);
    border-radius: 50px; /* 圆角更现代 */
    background: var(--bg-card);
    color: var(--text-main);
    font-size: 1rem;
    transition: all var(--transition-speed);
}

.search-input:focus {
    outline: none;
    border-color: var(--primary-color);
    box-shadow: 0 0 0 3px rgba(37, 99, 235, 0.1);
}

.search-icon {
    position: absolute;
    left: 18px;
    top: 50%;
    transform: translateY(-50%);
    color: var(--text-muted);
}

/* 筛选标签组 */
.filter-group {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-bottom: 2rem;
    padding-bottom: 1rem;
    border-bottom: 1px solid var(--border-color);
}

.filter-btn {
    background: transparent;
    border: 1px solid var(--border-color);
    color: var(--text-muted);
    padding: 6px 16px;
    border-radius: 20px;
    font-size: 0.9rem;
    cursor: pointer;
    transition: all var(--transition-speed);
    font-weight: 500;
}

.filter-btn:hover {
    background: var(--tag-bg);
    color: var(--text-main);
}

.filter-btn.active {
    background: var(--primary-color);
    color: white;
    border-color: var(--primary-color);
}

/* 论文列表容器 */
.pub-list {
    display: flex;
    flex-direction: column;
    gap: 1.5rem;
}

/* 论文卡片设计 - 更加学术、极简 */
.pub-card {
    background: var(--bg-card);
    border: 1px solid var(--border-color);
    border-radius: 8px;
    padding: 1.5rem;
    transition: transform var(--transition-speed), box-shadow var(--transition-speed);
    position: relative;
}

/* 仅在Hover时浮起，减少视觉干扰 */
.pub-card:hover {
    transform: translateY(-2px);
    box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.05);
    border-color: var(--primary-color);
}

.pub-header {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    gap: 1rem;
    margin-bottom: 0.5rem;
}

.pub-title {
    font-size: 1.15rem;
    font-weight: 700;
    color: var(--text-main);
    margin: 0;
    line-height: 1.4;
}

/* 奖项标记 */
.award-badge {
    display: inline-flex;
    align-items: center;
    gap: 4px;
    font-size: 0.8rem;
    color: var(--award-color);
    font-weight: 700;
    background: rgba(217, 119, 6, 0.1);
    padding: 2px 8px;
    border-radius: 4px;
    margin-top: 0.5rem;
    width: fit-content;
}

.pub-authors {
    color: var(--text-muted);
    font-size: 0.95rem;
    margin: 0.5rem 0;
    line-height: 1.5;
}

/* 作者名字高亮 */
.author-me {
    color: var(--text-main);
    font-weight: 700;
    text-decoration: underline;
    text-decoration-color: var(--primary-color);
    text-underline-offset: 3px;
}

.pub-venue {
    font-style: italic;
    color: var(--text-main);
    font-weight: 500;
}

.pub-meta {
    display: flex;
    gap: 10px;
    align-items: center;
    flex-wrap: wrap;
    font-size: 0.85rem;
    color: var(--text-muted);
    margin-bottom: 1rem;
}

.meta-tag {
    background: var(--tag-bg);
    padding: 2px 8px;
    border-radius: 4px;
}

/* 按钮组 - 统一风格 */
.pub-actions {
    display: flex;
    gap: 12px;
    flex-wrap: wrap;
    margin-top: 1rem;
}

.btn-action {
    display: inline-flex;
    align-items: center;
    gap: 6px;
    padding: 6px 12px;
    border-radius: 6px;
    font-size: 0.85rem;
    font-weight: 600;
    text-decoration: none;
    transition: all var(--transition-speed);
    border: 1px solid var(--border-color);
    color: var(--text-muted);
    background: transparent;
    cursor: pointer;
}

/* PDF/主按钮高亮 */
.btn-primary {
    color: var(--primary-color);
    border-color: var(--primary-color);
    background: rgba(37, 99, 235, 0.05);
}

.btn-action:hover {
    background: var(--tag-bg);
    color: var(--text-main);
}

.btn-primary:hover {
    background: var(--primary-color);
    color: white;
}

/* BibTeX 区域 */
.bibtex-container {
    margin-top: 1rem;
    background: var(--tag-bg);
    border-radius: 6px;
    padding: 1rem;
    font-family: 'Courier New', Courier, monospace;
    font-size: 0.8rem;
    overflow-x: auto;
    display: none; /* 默认隐藏 */
    position: relative;
    border: 1px solid var(--border-color);
    color: var(--text-main);
}

.bibtex-container.show {
    display: block;
    animation: fadeIn 0.3s ease;
}

.copy-feedback {
    position: absolute;
    top: 5px;
    right: 5px;
    background: #10b981;
    color: white;
    font-size: 0.7rem;
    padding: 2px 6px;
    border-radius: 4px;
    display: none;
}

@keyframes fadeIn {
    from { opacity: 0; transform: translateY(-5px); }
    to { opacity: 1; transform: translateY(0); }
}

/* 移动端优化 */
@media (max-width: 768px) {
    .stats-grid {
        grid-template-columns: repeat(2, 1fr);
    }
    .pub-header {
        flex-direction: column;
    }
}
</style>

<!-- 1. 统计面板 -->
<div class="pub-toolbar">
    <div class="stats-grid">
        <div class="stat-item">
            <h4 id="stat-total">15</h4>
            <p>Total Papers</p>
        </div>
        <div class="stat-item">
            <h4 id="stat-first">3</h4>
            <p>First Author</p>
        </div>
        <div class="stat-item">
            <h4>24.3</h4>
            <p>Max Impact Factor</p>
        </div>
        <div class="stat-item">
            <h4>250+</h4>
            <p>Citations</p>
        </div>
    </div>

    <!-- 2. 搜索框 -->
    <div class="search-wrapper">
        <i class="fa-solid fa-magnifying-glass search-icon"></i>
        <input type="text" id="searchInput" class="search-input" placeholder="Search by title, author, venue, or keywords...">
    </div>

    <!-- 3. 筛选器 -->
    <div class="filter-group" id="filterContainer">
        <button class="filter-btn active" data-filter="all">All</button>
        <button class="filter-btn" data-filter="selected">🔥 Selected</button>
        <button class="filter-btn" data-filter="2024">2024</button>
        <button class="filter-btn" data-filter="2023">2023</button>
        <button class="filter-btn" data-filter="journal">Journal</button>
        <button class="filter-btn" data-filter="conference">Conference</button>
        <button class="filter-btn" data-filter="cv">Computer Vision</button>
    </div>
</div>

<!-- 4. 论文列表 (无标题分割，纯时间倒序，通过Tag区分) -->
<div class="pub-list" id="publicationList">

    <!-- Paper 1 -->
    <article class="pub-card" data-year="2024" data-type="journal" data-tags="cv generative-ai selected" data-search="generative pretraining tpami mask">
        <div class="pub-header">
            <h3 class="pub-title">Towards Scalable Visual Representation Learning with Masked Generative Pretraining</h3>
            <span class="meta-tag" style="border: 1px solid var(--primary-color); color: var(--primary-color); font-weight: 600;">TPAMI 2024</span>
        </div>
        
        <div class="pub-authors">
            <span class="author-me">Your Name*</span>, Jane Smith, John Doe, Robert Brown
        </div>

        <div class="pub-venue">
            IEEE Transactions on Pattern Analysis and Machine Intelligence (TPAMI), In Press.
        </div>
        
        <div class="pub-meta">
            <span><i class="fa-solid fa-calendar"></i> 2024</span>
            <span><i class="fa-solid fa-chart-line"></i> IF: 24.314</span>
        </div>

        <div class="pub-actions">
            <a href="#" class="btn-action btn-primary"><i class="fa-solid fa-file-pdf"></i> PDF</a>
            <a href="#" class="btn-action"><i class="fa-brands fa-github"></i> Code</a>
            <a href="#" class="btn-action"><i class="fa-solid fa-globe"></i> Project</a>
            <button class="btn-action" onclick="toggleBibtex('bib1')"><i class="fa-solid fa-quote-right"></i> BibTeX</button>
        </div>

        <!-- Hidden BibTeX -->
        <div id="bib1" class="bibtex-container">
            <span class="copy-feedback">Copied!</span>
            <div class="code-content" onclick="copyBibtex('bib1')">
@article{name2024scalable,
  title={Towards Scalable Visual Representation Learning with Masked Generative Pretraining},
  author={Name, Your and Smith, Jane and Doe, John and Brown, Robert},
  journal={IEEE Transactions on Pattern Analysis and Machine Intelligence},
  year={2024},
  publisher={IEEE}
}
            </div>
            <div style="text-align: right; margin-top: 5px; color: var(--text-muted); font-size: 0.7rem;">Click to Copy</div>
        </div>
    </article>

    <!-- Paper 2 -->
    <article class="pub-card" data-year="2024" data-type="conference" data-tags="cv nerf selected" data-search="dynamic nerf view synthesis cvpr">
        <div class="pub-header">
            <h3 class="pub-title">Dynamic Neural Radiance Fields for Real-time View Synthesis</h3>
            <span class="meta-tag" style="border: 1px solid #8b5cf6; color: #8b5cf6; font-weight: 600;">CVPR 2024</span>
        </div>
        
        <div class="award-badge"><i class="fa-solid fa-trophy"></i> Oral Presentation (Top 3%)</div>

        <div class="pub-authors">
            <span class="author-me">Your Name*</span>, Carol Davis, Michael Lee (Equal Contribution)
        </div>

        <div class="pub-venue">
            IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR).
        </div>

        <div class="pub-actions">
            <a href="#" class="btn-action btn-primary"><i class="fa-solid fa-file-pdf"></i> PDF</a>
            <a href="#" class="btn-action"><i class="fa-solid fa-video"></i> Video</a>
            <a href="#" class="btn-action"><i class="fa-brands fa-github"></i> Code</a>
            <button class="btn-action" onclick="toggleBibtex('bib2')"><i class="fa-solid fa-quote-right"></i> BibTeX</button>
        </div>

        <div id="bib2" class="bibtex-container">
            <span class="copy-feedback">Copied!</span>
            <div class="code-content" onclick="copyBibtex('bib2')">
@inproceedings{name2024dynamic,
  title={Dynamic Neural Radiance Fields for Real-time View Synthesis},
  author={Name, Your and Davis, Carol and Lee, Michael},
  booktitle={CVPR},
  year={2024}
}
            </div>
        </div>
    </article>

    <!-- Paper 3 -->
    <article class="pub-card" data-year="2023" data-type="journal" data-tags="systems federated-learning" data-search="edge computing federated learning tist">
        <div class="pub-header">
            <h3 class="pub-title">Efficient Federated Learning for Edge Computing with Adaptive Client Selection</h3>
            <span class="meta-tag">ACM TIST 2023</span>
        </div>

        <div class="pub-authors">
            <span class="author-me">Your Name*</span>, Alice Johnson, Bob Wilson
        </div>

        <div class="pub-venue">
            ACM Transactions on Intelligent Systems and Technology.
        </div>
        
        <div class="pub-meta">
            <span><i class="fa-solid fa-calendar"></i> 2023</span>
            <a href="https://doi.org/10.1145/3582425" style="color: inherit; text-decoration: underline;"><i class="fa-solid fa-link"></i> DOI: 10.1145/3582425</a>
        </div>

        <div class="pub-actions">
            <a href="#" class="btn-action btn-primary"><i class="fa-solid fa-file-pdf"></i> PDF</a>
            <a href="#" class="btn-action"><i class="fa-brands fa-github"></i> Code</a>
            <button class="btn-action" onclick="toggleBibtex('bib3')"><i class="fa-solid fa-quote-right"></i> BibTeX</button>
        </div>

        <div id="bib3" class="bibtex-container">
            <span class="copy-feedback">Copied!</span>
            <div class="code-content" onclick="copyBibtex('bib3')">
@article{name2023efficient,
  title={Efficient Federated Learning for Edge Computing with Adaptive Client Selection},
  author={Name, Your and Johnson, Alice and Wilson, Bob},
  journal={ACM TIST},
  year={2023}
}
            </div>
        </div>
    </article>

</div>

<div style="margin-top: 3rem; text-align: center; color: var(--text-muted); font-size: 0.9rem;">
    <p>* indicates corresponding author. <br>
    Full publication list available on 
    <a href="#" class="author-me" style="text-decoration: none;">Google Scholar <i class="fa-solid fa-arrow-up-right-from-square" style="font-size: 0.7em;"></i></a>.</p>
</div>

<script>
/**
 * 核心功能逻辑
 * 1. 搜索过滤
 * 2. 按钮标签过滤
 * 3. BibTeX 显示与复制
 */

document.addEventListener('DOMContentLoaded', function() {
    const searchInput = document.getElementById('searchInput');
    const filterBtns = document.querySelectorAll('.filter-btn');
    const cards = document.querySelectorAll('.pub-card');
    
    // 当前激活的过滤器状态
    let activeFilter = 'all';
    
    // 1. 搜索功能
    searchInput.addEventListener('input', (e) => {
        const query = e.target.value.toLowerCase();
        filterPublications(activeFilter, query);
    });

    // 2. 标签点击筛选
    filterBtns.forEach(btn => {
        btn.addEventListener('click', () => {
            // 移除其他按钮激活状态
            filterBtns.forEach(b => b.classList.remove('active'));
            // 激活当前按钮
            btn.classList.add('active');
            
            activeFilter = btn.getAttribute('data-filter');
            const query = searchInput.value.toLowerCase();
            
            filterPublications(activeFilter, query);
        });
    });

    // 综合筛选函数
    function filterPublications(filter, query) {
        let visibleCount = 0;

        cards.forEach(card => {
            const year = card.getAttribute('data-year');
            const type = card.getAttribute('data-type');
            const tags = card.getAttribute('data-tags') || '';
            const searchData = (card.getAttribute('data-search') + ' ' + card.innerText).toLowerCase();

            // 检查标签匹配
            let matchesFilter = false;
            if (filter === 'all') matchesFilter = true;
            else if (filter === year) matchesFilter = true;
            else if (filter === type) matchesFilter = true;
            else if (tags.includes(filter)) matchesFilter = true;

            // 检查搜索匹配
            const matchesSearch = query === '' || searchData.includes(query);

            if (matchesFilter && matchesSearch) {
                card.style.display = 'block';
                // 简单的淡入动画
                card.style.opacity = '0';
                setTimeout(() => card.style.opacity = '1', 50);
                visibleCount++;
            } else {
                card.style.display = 'none';
            }
        });
        
        // 可选：如果没有任何结果显示提示信息 (此处略)
    }
});

// 3. BibTeX 切换显示
function toggleBibtex(id) {
    const el = document.getElementById(id);
    if (el.classList.contains('show')) {
        el.classList.remove('show');
        setTimeout(() => el.style.display = 'none', 300); // 等待动画结束
    } else {
        el.style.display = 'block';
        // 强制重绘以触发 transition
        setTimeout(() => el.classList.add('show'), 10);
    }
}

// 4. BibTeX 复制功能
function copyBibtex(id) {
    const container = document.getElementById(id);
    const code = container.querySelector('.code-content').innerText;
    
    navigator.clipboard.writeText(code).then(() => {
        const feedback = container.querySelector('.copy-feedback');
        feedback.style.display = 'block';
        setTimeout(() => {
            feedback.style.display = 'none';
        }, 2000);
    }).catch(err => {
        console.error('Failed to copy: ', err);
    });
}
</script>