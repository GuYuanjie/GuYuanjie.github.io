---
title: "Publications"
description: "Selected peer-reviewed journals and conference proceedings."
layout: "simple"
fullWidth: true
---

<!-- 引入 FontAwesome 图标库 -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

{{< publications_css >}}

<div class="pub-toolbar">
    {{< publications_stats >}}
    
    {{< publications_search >}}
</div>

<!-- 论文列表 -->
<div class="pub-list" id="publicationList">

    <!-- Paper 1 -->
    {{< publication_item
        title="Towards Scalable Visual Representation Learning with Masked Generative Pretraining"
        year="2024"
        type="journal"
        tags="cv generative-ai selected"
        search="generative pretraining tpami mask"
        authors="<span class='author-me'>Your Name*</span>, Jane Smith, John Doe, Robert Brown"
        venue="IEEE Transactions on Pattern Analysis and Machine Intelligence (TPAMI), In Press."
        meta="<span><i class='fa-solid fa-calendar'></i> 2024</span><span><i class='fa-solid fa-chart-line'></i> IF: 24.314</span>"
        venueStyle="border: 1px solid var(--primary-color); color: var(--primary-color);"
        bibtexId="bib1"
        bibtex=`@article{name2024scalable,
  title={Towards Scalable Visual Representation Learning with Masked Generative Pretraining},
  author={Name, Your and Smith, Jane and Doe, John and Brown, Robert},
  journal={IEEE Transactions on Pattern Analysis and Machine Intelligence},
  year={2024},
  publisher={IEEE}
}`
    >}}
    <a href="#" class="btn-action btn-primary"><i class="fa-solid fa-file-pdf"></i> PDF</a>
    <a href="#" class="btn-action"><i class="fa-brands fa-github"></i> Code</a>
    <a href="#" class="btn-action"><i class="fa-solid fa-globe"></i> Project</a>
    <button class="btn-action" onclick="toggleBibtex('bib1')"><i class="fa-solid fa-quote-right"></i> BibTeX</button>
    {{< /publication_item >}}

    <!-- Paper 2 -->
    {{< publication_item
        title="Dynamic Neural Radiance Fields for Real-time View Synthesis"
        year="2024"
        type="conference"
        tags="cv nerf selected"
        search="dynamic nerf view synthesis cvpr"
        authors="<span class='author-me'>Your Name*</span>, Carol Davis, Michael Lee (Equal Contribution)"
        venue="IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)."
        award="Oral Presentation (Top 3%)"
        venueStyle="border: 1px solid #8b5cf6; color: #8b5cf6;"
        bibtexId="bib2"
        bibtex=`@inproceedings{name2024dynamic,
  title={Dynamic Neural Radiance Fields for Real-time View Synthesis},
  author={Name, Your and Davis, Carol and Lee, Michael},
  booktitle={CVPR},
  year={2024}
}`
    >}}
    <a href="#" class="btn-action btn-primary"><i class="fa-solid fa-file-pdf"></i> PDF</a>
    <a href="#" class="btn-action"><i class="fa-solid fa-video"></i> Video</a>
    <a href="#" class="btn-action"><i class="fa-brands fa-github"></i> Code</a>
    <button class="btn-action" onclick="toggleBibtex('bib2')"><i class="fa-solid fa-quote-right"></i> BibTeX</button>
    {{< /publication_item >}}

    <!-- Paper 3 -->
    {{< publication_item
        title="Efficient Federated Learning for Edge Computing with Adaptive Client Selection"
        year="2023"
        type="journal"
        tags="systems federated-learning"
        search="edge computing federated learning tist"
        authors="<span class='author-me'>Your Name*</span>, Alice Johnson, Bob Wilson"
        venue="ACM Transactions on Intelligent Systems and Technology."
        meta="<span><i class='fa-solid fa-calendar'></i> 2023</span><a href='https://doi.org/10.1145/3582425' style='color: inherit; text-decoration: underline;'><i class='fa-solid fa-link'></i> DOI: 10.1145/3582425</a>"
        bibtexId="bib3"
        bibtex=`@article{name2023efficient,
  title={Efficient Federated Learning for Edge Computing with Adaptive Client Selection},
  author={Name, Your and Johnson, Alice and Wilson, Bob},
  journal={ACM TIST},
  year={2023}
}`
    >}}
    <a href="#" class="btn-action btn-primary"><i class="fa-solid fa-file-pdf"></i> PDF</a>
    <a href="#" class="btn-action"><i class="fa-brands fa-github"></i> Code</a>
    <button class="btn-action" onclick="toggleBibtex('bib3')"><i class="fa-solid fa-quote-right"></i> BibTeX</button>
    {{< /publication_item >}}

</div>

<div style="margin-top: 3rem; text-align: center; color: var(--text-muted); font-size: 0.9rem;">
    <p>* indicates corresponding author. <br>
    Full publication list available on 
    <a href="#" class="author-me" style="text-decoration: none;">Google Scholar <i class="fa-solid fa-arrow-up-right-from-square" style="font-size: 0.7em;"></i></a>.</p>
</div>

{{< publications_js >}}