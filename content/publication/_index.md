---
title: "Publications"
layout: "simple"
fullWidth: true
---

<!-- 引入 FontAwesome -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

{{< publications_css >}}

<!-- 统计栏：会自动变成 2x2 (手机) 或 1x4 (电脑) -->
{{< publications_stats >}}

{{< publications_search >}}

<!-- 文章列表：CSS Grid 布局，每行一个 Card，紧凑排列 -->
<div class="pub-list" id="publicationList">

<!-- Card 1 -->
    {{< publication_item
        title="Towards Scalable Visual Representation Learning"
        year="2024"
        type="journal"
        tags="cv selected"
        authors="<span class='author-me'>Your Name</span>, et al."
        venue="IEEE TPAMI"
        meta="<span>2024</span><span>IF: 24.3</span>"
        venueStyle="border: 1px solid var(--pub-primary); color: var(--pub-primary);"
        bibtexId="bib1"
        bibtex="@article{...}"
    >}}
    <a href="#" class="btn-action btn-primary">PDF</a>
    <a href="#" class="btn-action">Code</a>
    {{< /publication_item >}}
    
<!-- Card 2 -->
    {{< publication_item
        title="Another Paper Title"
        year="2023"
        type="conference"
        tags="cv"
        authors="Author A, <span class='author-me'>Your Name</span>"
        venue="CVPR 2023"
        meta="<span>2023</span>"
        bibtexId="bib2"
        bibtex="@inproceedings{...}"
    >}}
    <a href="#" class="btn-action btn-primary">PDF</a>
    {{< /publication_item >}}

    <!-- Card 2 -->
    {{< publication_item
        title="Another Paper Title"
        year="2023"
        type="conference"
        tags="cv"
        authors="Author A, <span class='author-me'>Your Name</span>"
        venue="CVPR 2023"
        meta="<span>2023</span>"
        bibtexId="bib2"
        bibtex="@inproceedings{...}"
    >}}
    <a href="#" class="btn-action btn-primary">PDF</a>
    {{< /publication_item >}}


<!-- Card 2 -->
    {{< publication_item
        title="Another Paper Title"
        year="2023"
        type="conference"
        tags="cv"
        authors="Author A, <span class='author-me'>Your Name</span>"
        venue="CVPR 2023"
        meta="<span>2023</span>"
        bibtexId="bib2"
        bibtex="@inproceedings{...}"
    >}}
    <a href="#" class="btn-action btn-primary">PDF</a>
    {{< /publication_item >}}


<!-- Card 2 -->
    {{< publication_item
        title="Another Paper Title"
        year="2023"
        type="conference"
        tags="cv"
        authors="Author A, <span class='author-me'>Your Name</span>"
        venue="CVPR 2023"
        meta="<span>2023</span>"
        bibtexId="bib2"
        bibtex="@inproceedings{...}"
    >}}
    <a href="#" class="btn-action btn-primary">PDF</a>
    {{< /publication_item >}}


</div>

{{< publications_js >}}