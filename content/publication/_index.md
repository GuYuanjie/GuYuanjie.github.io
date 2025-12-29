---
title: "Publications"
layout: "simple"
fullWidth: true
---

<!-- 引入 FontAwesome -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<div class="pub-content">

<!-- 统计栏 -->
{{< publications_stats 
    total="15" 
    first="3" 
    impact="24.3" 
    citations="250+" 
>}}

<!-- 搜索和筛选 -->
{{< publications_search >}}

<!-- 论文列表 -->
<div class="pub-list" id="publicationList">

      <!-- 示例1 -->
      {{< publication_item
          title="Towards Scalable Visual Representation Learning"
          year="2024"
          type="journal"
          tags="cv,selected"
          search="vision transformer deep learning"
          authors="<span class='author-me'>Your Name</span>, Jane Smith, John Doe"
          venue="IEEE Transactions on Pattern Analysis and Machine Intelligence (TPAMI)"
          award="Best Paper Award"
          meta="<span><i class='fas fa-calendar'></i> 2024</span><span><i class='fas fa-star'></i> Impact: 24.3</span><span><i class='fas fa-quote-right'></i> Citations: 150</span>"
          venueStyle="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white;"
          bibtexId="bib1"
          bibtex="@article{example2024,&#10;  title={Towards Scalable Visual Representation Learning},&#10;  author={Your Name and Jane Smith and John Doe},&#10;  journal={IEEE Transactions on Pattern Analysis and Machine Intelligence},&#10;  volume={46},&#10;  number={1},&#10;  pages={1--15},&#10;  year={2024},&#10;  publisher={IEEE}&#10;}"
      >}}
          <a href="https://example.com/paper.pdf" class="btn-action btn-primary">
              <i class="fas fa-file-pdf"></i> PDF
          </a>
          <a href="https://github.com/example/code" class="btn-action">
              <i class="fab fa-github"></i> Code
          </a>
          <button class="btn-action" onclick="toggleBibtex('bib1')">
              <i class="fas fa-quote-right"></i> BibTeX
          </button>
          <a href="https://arxiv.org/abs/xxxx.xxxxx" class="btn-action">
              <i class="fas fa-external-link-alt"></i> arXiv
          </a>
      {{< /publication_item >}}

      <!-- 示例2 -->
      {{< publication_item
          title="Efficient Multi-Modal Learning for Visual Recognition"
          year="2023"
          type="conference"
          tags="cv,multimodal"
          search="multimodal attention efficient"
          authors="Alice Johnson, <span class='author-me'>Your Name</span>, Bob Wilson"
          venue="International Conference on Computer Vision and Pattern Recognition (CVPR)"
          meta="<span><i class='fas fa-calendar'></i> 2023</span><span><i class='fas fa-quote-right'></i> Citations: 85</span>"
          bibtexId="bib2"
          bibtex="@inproceedings{example2023,&#10;  title={Efficient Multi-Modal Learning for Visual Recognition},&#10;  author={Alice Johnson and Your Name and Bob Wilson},&#10;  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},&#10;  pages={12345--12355},&#10;  year={2023}&#10;}"
      >}}
          <a href="https://example.com/paper2.pdf" class="btn-action btn-primary">
              <i class="fas fa-file-pdf"></i> PDF
          </a>
          <a href="https://github.com/example/multimodal" class="btn-action">
              <i class="fab fa-github"></i> Code
          </a>
          <button class="btn-action" onclick="toggleBibtex('bib2')">
              <i class="fas fa-quote-right"></i> BibTeX
          </button>
      {{< /publication_item >}}

</div>

</div>

<!-- 添加 toggleBibtex 函数 -->
<script>
function toggleBibtex(id) {
    const el = document.getElementById(id);
    if (!el) return;
    
    if (el.classList.contains('show')) {
        el.classList.remove('show');
        setTimeout(() => el.style.display = 'none', 300);
    } else {
        el.style.display = 'block';
        setTimeout(() => el.classList.add('show'), 10);
    }
}
</script>