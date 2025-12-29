---
title: "Publications"
layout: "simple"
fullWidth: true
---

<!-- 引入 FontAwesome -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<!-- 引入自定义样式 -->
{{< publications_css >}}

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
        bibtex="@article{example2024, title={Towards Scalable Visual Representation Learning}, author={Your Name and Jane Smith and John Doe}, journal={IEEE Transactions on Pattern Analysis and Machine Intelligence}, volume={46}, number={1}, pages={1--15}, year={2024}, publisher={IEEE}}"
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
        bibtex="@inproceedings{example2023, title={Efficient Multi-Modal Learning for Visual Recognition}, author={Alice Johnson and Your Name and Bob Wilson}, booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition}, pages={12345--12355}, year={2023}}"
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

<!-- 引入 JavaScript -->
{{< publications_js >}}