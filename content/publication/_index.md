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

<!-- 统计栏 (数据需根据实际情况微调) -->
{{< publications_stats 
    total="17" 
    first="8" 
    impact="100+" 
    citations="50+" 
>}}

<!-- 搜索和筛选 -->
{{< publications_search >}}

<!-- 论文列表 -->
<div class="pub-list" id="publicationList">
    <!-- ================================================================================== -->
    <!-- 2025 Papers -->
    <!-- ================================================================================== -->
    {{< publication_item
        title="Enhancing Biomedical Optical Volumetric Imaging via Self-Supervised Orthogonal Learning"
        year="2025"
        type="journal"
        tags="ai,imaging,selected"
        search="self-supervised biomedical optical imaging"
        authors="<span class='author-me'>Yuanjie Gu</span>, Yiqun Wang, Ang Xuan, Jianping Wang, Linyi Wang, Lei Zhang, Xiaoran Li, Yao Wu, Jun Zhang, Zhi Lu, Biqin Dong"
        venue="Science Advances"
        venueStyle="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white;"
        meta="<span><i class='fas fa-calendar'></i> 2025</span><span><i class='fas fa-book'></i> Sci. Adv.</span><span><i class='fas fa-star'></i> IF: ~11.6</span><span><i class='fas fa-info-circle'></i> Minor Revision</span>"
        bibtexId="bib1"
        bibtexKey="gu2025enhancing"
        bibtexContent="@article{gu2025enhancing, title={Enhancing Biomedical Optical Volumetric Imaging via Self-Supervised Orthogonal Learning}, author={Gu, Yuanjie and Wang, Yiqun and Xuan, Ang and Wang, Jianping and Wang, Linyi and Zhang, Lei and Li, Xiaoran and Wu, Yao and Zhang, Jun and Lu, Zhi and Dong, Biqin}, journal={Science Advances}, year={2025}}"
    >}}
        <a href="#" class="btn-action btn-primary"><i class="fas fa-file-pdf"></i> PDF</a>
        <a href="#" class="btn-action"><i class="fab fa-github"></i> Code</a>
        <button class="btn-action" onclick="toggleBibtex('bib1')"><i class="fas fa-quote-right"></i> BibTeX</button>
        <a href="https://www.biorxiv.org/content/10.1101/2025.05.16.654259v1" class="btn-action"><i class="fas fa-external-link-alt"></i> bioRxiv</a>
    {{< /publication_item >}}
    {{< publication_item
        title="Real-time Self-supervised Denoising for High-speed Fluorescence Neural Imaging"
        year="2025"
        type="journal"
        tags="ai,neuroscience,selected"
        search="real-time self-supervised denoising neural imaging"
        authors="Yiqun Wang, <span class='author-me'>Yuanjie Gu</span>, Jianping Wang, Ang Xuan, Cihang Kong, Wei-Qun Fang, Dongyu Li, Dan Zhu, Fengfei Ding, Biqin Dong"
        venue="Nature Communications"
        venueStyle="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white;"
        meta="<span><i class='fas fa-calendar'></i> 2025</span><span><i class='fas fa-book'></i> Nat. Commun.</span><span><i class='fas fa-star'></i> IF: ~14.7</span><span><i class='fas fa-quote-right'></i> Citations: TBD</span>"
        bibtexId="bib2"
        bibtexKey="wang2025realtime"
        bibtexContent="@article{wang2025realtime, title={Real-time Self-supervised Denoising for High-speed Fluorescence Neural Imaging}, author={Wang, Yiqun and Gu, Yuanjie and Wang, Jianping and Xuan, Ang and Kong, Cihang and Fang, Wei-Qun and Li, Dongyu and Zhu, Dan and Ding, Fengfei and Dong, Biqin}, journal={Nature Communications}, volume={16}, pages={9396}, year={2025}}"
    >}}
        <a href="#" class="btn-action btn-primary"><i class="fas fa-file-pdf"></i> PDF</a>
        <a href="#" class="btn-action"><i class="fab fa-github"></i> Code</a>
        <button class="btn-action" onclick="toggleBibtex('bib2')"><i class="fas fa-quote-right"></i> BibTeX</button>
        <a href="#" class="btn-action"><i class="fas fa-external-link-alt"></i> arXiv</a>
    {{< /publication_item >}}
    {{< publication_item
        title="GaMA: Stochastic Gaussian-masked Denoiser for Enhanced Fluorescence Microscopy of Subcellular Structures and Neural Dynamics"
        year="2025"
        type="journal"
        tags="ai,microscopy"
        search="fluorescence microscopy denoising neural dynamics"
        authors="<span class='author-me'>Yuanjie Gu</span>, Yiqun Wang, Zhenyao Zhao, Jun Lu, Lei Xu, Zhi Lu, Biqin Dong"
        venue="Advanced Technology in Neuroscience"
        meta="<span><i class='fas fa-calendar'></i> 2025</span><span><i class='fas fa-book'></i> Adv. Tech. Neurosci.</span><span><i class='fas fa-star'></i> IF: TBD</span><span><i class='fas fa-quote-right'></i> Citations: TBD</span>"
        bibtexId="bib3"
        bibtexKey="gu2025gama"
        bibtexContent="@article{gu2025gama, title={GaMA: Stochastic Gaussian-masked Denoiser for Enhanced Fluorescence Microscopy of Subcellular Structures and Neural Dynamics}, author={Gu, Yuanjie and Wang, Yiqun and Zhao, Zhenyao and Lu, Jun and Xu, Lei and Lu, Zhi and Dong, Biqin}, journal={Advanced Technology in Neuroscience}, volume={3}, pages={1-5}, year={2025}}"
    >}}
        <a href="#" class="btn-action btn-primary"><i class="fas fa-file-pdf"></i> PDF</a>
        <a href="#" class="btn-action"><i class="fab fa-github"></i> Code</a>
        <button class="btn-action" onclick="toggleBibtex('bib3')"><i class="fas fa-quote-right"></i> BibTeX</button>
        <a href="#" class="btn-action"><i class="fas fa-external-link-alt"></i> arXiv</a>
    {{< /publication_item >}}
    {{< publication_item
        title="Automated Enhanced Handheld Fundus Photography via Unpaired Learning"
        year="2025"
        type="journal"
        tags="ai,medical imaging"
        search="fundus photography unpaired learning enhancement"
        authors="<span class='author-me'>Yuanjie Gu</span>, Jiacheng Yang, Yiqun Wang, Mengwen Ye, Xin Li, Xiaoran Li, Na Li, Jun Zhang, Yitian Zhao, Zekuan Yu, Biqin Dong"
        venue="IEEE Transactions on Instrumentation & Measurement"
        meta="<span><i class='fas fa-calendar'></i> 2025</span><span><i class='fas fa-book'></i> IEEE TIM</span><span><i class='fas fa-star'></i> IF: ~5.6</span><span><i class='fas fa-quote-right'></i> Citations: TBD</span>"
        bibtexId="bib4"
        bibtexKey="gu2025automated"
        bibtexContent="@article{gu2025automated, title={Automated Enhanced Handheld Fundus Photography via Unpaired Learning}, author={Gu, Yuanjie and Yang, Jiacheng and Wang, Yiqun and Ye, Mengwen and Li, Xin and Li, Xiaoran and Li, Na and Zhang, Jun and Zhao, Yitian and Yu, Zekuan and Dong, Biqin}, journal={IEEE Transactions on Instrumentation and Measurement}, volume={74}, pages={1-12}, year={2025}}"
    >}}
        <a href="#" class="btn-action btn-primary"><i class="fas fa-file-pdf"></i> PDF</a>
        <a href="#" class="btn-action"><i class="fab fa-github"></i> Code</a>
        <button class="btn-action" onclick="toggleBibtex('bib4')"><i class="fas fa-quote-right"></i> BibTeX</button>
        <a href="#" class="btn-action"><i class="fas fa-external-link-alt"></i> arXiv</a>
    {{< /publication_item >}}
    {{< publication_item
        title="Automated Diagnosis of Non-Melanoma Skin Cancer: A Joint Learning Approach Using Optical Attenuation Coefficients"
        year="2025"
        type="journal"
        tags="ai,medical"
        search="skin cancer diagnosis optical attenuation"
        authors="Lei Zhang, Xiaoran Li, Wen Chen, <span class='author-me'>Yuanjie Gu</span>, Hao Wu, Zhong Lu, Biqin Dong"
        venue="npj Digital Medicine"
        meta="<span><i class='fas fa-calendar'></i> 2025</span><span><i class='fas fa-book'></i> npj Dig. Med.</span><span><i class='fas fa-star'></i> IF: ~15.0</span><span><i class='fas fa-quote-right'></i> Citations: TBD</span>"
        bibtexId="bib13"
        bibtexKey="zhang2025automated"
        bibtexContent="@article{zhang2025automated, title={Automated Diagnosis of Non-Melanoma Skin Cancer: A Joint Learning Approach Using Optical Attenuation Coefficients}, author={Zhang, Lei and Li, Xiaoran and Chen, Wen and Gu, Yuanjie and Wu, Hao and Lu, Zhong and Dong, Biqin}, journal={npj Digital Medicine}, volume={8}, pages={232}, year={2025}}"
    >}}
        <a href="#" class="btn-action btn-primary"><i class="fas fa-file-pdf"></i> PDF</a>
        <a href="#" class="btn-action"><i class="fab fa-github"></i> Code</a>
        <button class="btn-action" onclick="toggleBibtex('bib13')"><i class="fas fa-quote-right"></i> BibTeX</button>
        <a href="#" class="btn-action"><i class="fas fa-external-link-alt"></i> arXiv</a>
    {{< /publication_item >}}
    {{< publication_item
        title="Fed-GFM-DG: A Privacy-Preserving Framework for Fundus Image Segmentation via Generative-based Feature Generalization and Mask-Guided Aggregation"
        year="2025"
        type="journal"
        tags="ai,federated learning"
        search="federated learning fundus image segmentation"
        authors="Jiacheng Yang, <span class='author-me'>Yuanjie Gu</span>, Shujian Gao, Wei Ren, Zekuan Yu"
        venue="Biomedical Signal Processing and Control"
        meta="<span><i class='fas fa-calendar'></i> 2025</span><span><i class='fas fa-book'></i> BSPC</span><span><i class='fas fa-star'></i> IF: ~5.1</span><span><i class='fas fa-quote-right'></i> Citations: TBD</span>"
        bibtexId="bib14"
        bibtexKey="yang2025fedgfm"
        bibtexContent="@article{yang2025fedgfm, title={Fed-GFM-DG: A Privacy-Preserving Framework for Fundus Image Segmentation via Generative-based Feature Generalization and Mask-Guided Aggregation}, author={Yang, Jiacheng and Gu, Yuanjie and Gao, Shujian and Ren, Wei and Yu, Zekuan}, journal={Biomedical Signal Processing and Control}, volume={106}, pages={1-14}, year={2025}}"
    >}}
        <a href="#" class="btn-action btn-primary"><i class="fas fa-file-pdf"></i> PDF</a>
        <a href="#" class="btn-action"><i class="fab fa-github"></i> Code</a>
        <button class="btn-action" onclick="toggleBibtex('bib14')"><i class="fas fa-quote-right"></i> BibTeX</button>
        <a href="#" class="btn-action"><i class="fas fa-external-link-alt"></i> arXiv</a>
    {{< /publication_item >}}
    <!-- ================================================================================== -->
    <!-- 2024 Papers -->
    <!-- ================================================================================== -->
    {{< publication_item
        title="Deep-learning-assisted spectroscopic single-molecule localization microscopy based on spectrum-to-spectrum denoising"
        year="2024"
        type="journal"
        tags="ai,microscopy"
        search="single-molecule localization microscopy denoising"
        authors="Dandan Xu, <span class='author-me'>Yuanjie Gu</span>, Jun Lu, Lei Xu, Wei Wang, Biqin Dong"
        venue="Nanoscale"
        meta="<span><i class='fas fa-calendar'></i> 2024</span><span><i class='fas fa-book'></i> Nanoscale</span><span><i class='fas fa-star'></i> IF: ~6.7</span><span><i class='fas fa-quote-right'></i> Citations: TBD</span>"
        bibtexId="bib15"
        bibtexKey="xu2024deeplearning"
        bibtexContent="@article{xu2024deeplearning, title={Deep-learning-assisted spectroscopic single-molecule localization microscopy based on spectrum-to-spectrum denoising}, author={Xu, Dandan and Gu, Yuanjie and Lu, Jun and Xu, Lei and Wang, Wei and Dong, Biqin}, journal={Nanoscale}, volume={16}, number={11}, pages={5729-5736}, year={2024}}"
    >}}
        <a href="#" class="btn-action btn-primary"><i class="fas fa-file-pdf"></i> PDF</a>
        <a href="#" class="btn-action"><i class="fab fa-github"></i> Code</a>
        <button class="btn-action" onclick="toggleBibtex('bib15')"><i class="fas fa-quote-right"></i> BibTeX</button>
        <a href="#" class="btn-action"><i class="fas fa-external-link-alt"></i> arXiv</a>
    {{< /publication_item >}}
    {{< publication_item
        title="Super Resolution Reconstruction of Fluorescence Microscopy Image by Convolutional Network with Physical Priors"
        year="2024"
        type="journal"
        tags="ai,imaging"
        search="super-resolution fluorescence microscopy physical priors"
        authors="Qiangyu Cai, Jun Lu, Wenting Gu, Di Xiao, Boyi Li, Lei Xu, <span class='author-me'>Yuanjie Gu</span>, Biqin Dong, Xin Liu"
        venue="Biomedical Optics Express"
        meta="<span><i class='fas fa-calendar'></i> 2024</span><span><i class='fas fa-book'></i> BOE</span><span><i class='fas fa-star'></i> IF: ~3.4</span><span><i class='fas fa-quote-right'></i> Citations: TBD</span>"
        bibtexId="bib16"
        bibtexKey="cai2024super"
        bibtexContent="@article{cai2024super, title={Super Resolution Reconstruction of Fluorescence Microscopy Image by Convolutional Network with Physical Priors}, author={Cai, Qiangyu and Lu, Jun and Gu, Wenting and Xiao, Di and Li, Boyi and Xu, Lei and Gu, Yuanjie and Dong, Biqin and Liu, Xin}, journal={Biomedical Optics Express}, volume={15}, number={11}, pages={6638-6653}, year={2024}}"
    >}}
        <a href="#" class="btn-action btn-primary"><i class="fas fa-file-pdf"></i> PDF</a>
        <a href="#" class="btn-action"><i class="fab fa-github"></i> Code</a>
        <button class="btn-action" onclick="toggleBibtex('bib16')"><i class="fas fa-quote-right"></i> BibTeX</button>
        <a href="#" class="btn-action"><i class="fas fa-external-link-alt"></i> arXiv</a>
    {{< /publication_item >}}
    <!-- ================================================================================== -->
    <!-- 2023 Papers -->
    <!-- ================================================================================== -->
    {{< publication_item
        title="SegCoFusion: An Integrative Multimodal Volumetric Segmentation Cooperating with Fusion Pipeline to Enhance Lesion Awareness"
        year="2023"
        type="journal"
        tags="ai,segmentation"
        search="multimodal volumetric segmentation lesion awareness"
        authors="<span class='author-me'>Yuanjie Gu</span>, Yinghan Guan, Zekuan Yu, Biqin Dong"
        venue="IEEE Journal of Biomedical and Health Informatics"
        meta="<span><i class='fas fa-calendar'></i> 2023</span><span><i class='fas fa-book'></i> IEEE JBHI</span><span><i class='fas fa-star'></i> IF: ~7.7</span><span><i class='fas fa-quote-right'></i> Citations: TBD</span>"
        bibtexId="bib5"
        bibtexKey="gu2023segcofusion"
        bibtexContent="@article{gu2023segcofusion, title={SegCoFusion: An Integrative Multimodal Volumetric Segmentation Cooperating with Fusion Pipeline to Enhance Lesion Awareness}, author={Gu, Yuanjie and Guan, Yinghan and Yu, Zekuan and Dong, Biqin}, journal={IEEE Journal of Biomedical and Health Informatics}, volume={27}, number={12}, pages={5860-5871}, year={2023}}"
    >}}
        <a href="#" class="btn-action btn-primary"><i class="fas fa-file-pdf"></i> PDF</a>
        <a href="#" class="btn-action"><i class="fab fa-github"></i> Code</a>
        <button class="btn-action" onclick="toggleBibtex('bib5')"><i class="fas fa-quote-right"></i> BibTeX</button>
        <a href="#" class="btn-action"><i class="fas fa-external-link-alt"></i> arXiv</a>
    {{< /publication_item >}}
    {{< publication_item
        title="Physics Driven Deep Retinex Fusion for Adaptive Infrared and Visible Image Fusion"
        year="2023"
        type="journal"
        tags="ai,image fusion"
        award="SPIE Wechat Highlight Paper"
        search="infrared visible image fusion retinex"
        authors="<span class='author-me'>Yuanjie Gu</span>, Zhibo Xiao, Yinghan Guan, Haoran Dai, Cheng Liu, Liang Xue, Shouyu Wang"
        venue="Optical Engineering"
        meta="<span><i class='fas fa-calendar'></i> 2023</span><span><i class='fas fa-book'></i> Opt. Eng.</span><span><i class='fas fa-star'></i> IF: ~1.3</span><span><i class='fas fa-quote-right'></i> Citations: TBD</span>"
        bibtexId="bib7"
        bibtexKey="gu2023physics"
        bibtexContent="@article{gu2023physics, title={Physics Driven Deep Retinex Fusion for Adaptive Infrared and Visible Image Fusion}, author={Gu, Yuanjie and Xiao, Zhibo and Guan, Yinghan and Dai, Haoran and Liu, Cheng and Xue, Liang and Wang, Shouyu}, journal={Optical Engineering}, volume={62}, number={8}, pages={083101}, year={2023}}"
    >}}
        <a href="#" class="btn-action btn-primary"><i class="fas fa-file-pdf"></i> PDF</a>
        <a href="#" class="btn-action"><i class="fab fa-github"></i> Code</a>
        <button class="btn-action" onclick="toggleBibtex('bib7')"><i class="fas fa-quote-right"></i> BibTeX</button>
        <a href="#" class="btn-action"><i class="fas fa-external-link-alt"></i> arXiv</a>
    {{< /publication_item >}}
    {{< publication_item
        title="Deep SBP+: Breaking Through the Space-bandwidth Product Limit based on a Physical-driven Cycle Constraint Framework"
        year="2023"
        type="journal"
        tags="ai,imaging"
        search="space-bandwidth product limit cycle constraint"
        authors="Zhibo Xiao, <span class='author-me'>Yuanjie Gu</span>, Lin Zhu, Cheng Liu, Shouyu Wang"
        venue="Journal of the Optical Society of America A"
        meta="<span><i class='fas fa-calendar'></i> 2023</span><span><i class='fas fa-book'></i> JOSA A</span><span><i class='fas fa-star'></i> IF: ~1.8</span><span><i class='fas fa-quote-right'></i> Citations: TBD</span>"
        bibtexId="bib10"
        bibtexKey="xiao2023deep"
        bibtexContent="@article{xiao2023deep, title={Deep SBP+: Breaking Through the Space-bandwidth Product Limit based on a Physical-driven Cycle Constraint Framework}, author={Xiao, Zhibo and Gu, Yuanjie and Zhu, Lin and Liu, Cheng and Wang, Shouyu}, journal={Journal of the Optical Society of America A}, volume={40}, number={5}, pages={833-840}, year={2023}}"
    >}}
        <a href="#" class="btn-action btn-primary"><i class="fas fa-file-pdf"></i> PDF</a>
        <a href="#" class="btn-action"><i class="fab fa-github"></i> Code</a>
        <button class="btn-action" onclick="toggleBibtex('bib10')"><i class="fas fa-quote-right"></i> BibTeX</button>
        <a href="#" class="btn-action"><i class="fas fa-external-link-alt"></i> arXiv</a>
    {{< /publication_item >}}
    {{< publication_item
        title="Deep-Gamma: Deep Low-excitation Fluorescence Imaging Global Enhancement"
        year="2023"
        type="journal"
        tags="ai,imaging"
        search="fluorescence imaging global enhancement deep learning"
        authors="Zhibo Xiao, Yinghan Guan, Wei Hou, <span class='author-me'>Yuanjie Gu</span>, Shouyu Wang"
        venue="Optics Letters"
        meta="<span><i class='fas fa-calendar'></i> 2023</span><span><i class='fas fa-book'></i> Opt. Lett.</span><span><i class='fas fa-star'></i> IF: ~3.6</span><span><i class='fas fa-quote-right'></i> Citations: TBD</span>"
        bibtexId="bib12"
        bibtexKey="xiao2023deepgamma"
        bibtexContent="@article{xiao2023deepgamma, title={Deep-Gamma: Deep Low-excitation Fluorescence Imaging Global Enhancement}, author={Xiao, Zhibo and Guan, Yinghan and Hou, Wei and Gu, Yuanjie and Wang, Shouyu}, journal={Optics Letters}, volume={48}, number={9}, pages={2496-2499}, year={2023}}"
    >}}
        <a href="#" class="btn-action btn-primary"><i class="fas fa-file-pdf"></i> PDF</a>
        <a href="#" class="btn-action"><i class="fab fa-github"></i> Code</a>
        <button class="btn-action" onclick="toggleBibtex('bib12')"><i class="fas fa-quote-right"></i> BibTeX</button>
        <a href="#" class="btn-action"><i class="fas fa-external-link-alt"></i> arXiv</a>
    {{< /publication_item >}}
    <!-- ================================================================================== -->
    <!-- 2022 Papers -->
    <!-- ================================================================================== -->
    {{< publication_item
        title="Deep Low-excitation Fluorescence Imaging Enhancement"
        year="2022"
        type="journal"
        tags="ai,imaging"
        search="fluorescence imaging enhancement low-excitation"
        authors="<span class='author-me'>Yuanjie Gu</span>, Zhibo Xiao, Wei Hou, Cheng Liu, Ying Jin, Shouyu Wang"
        venue="Optics Letters"
        meta="<span><i class='fas fa-calendar'></i> 2022</span><span><i class='fas fa-book'></i> Opt. Lett.</span><span><i class='fas fa-star'></i> IF: ~3.6</span><span><i class='fas fa-quote-right'></i> Citations: TBD</span>"
        bibtexId="bib6"
        bibtexKey="gu2022deep"
        bibtexContent="@article{gu2022deep, title={Deep Low-excitation Fluorescence Imaging Enhancement}, author={Gu, Yuanjie and Xiao, Zhibo and Hou, Wei and Liu, Cheng and Jin, Ying and Wang, Shouyu}, journal={Optics Letters}, volume={47}, number={16}, pages={4175-4178}, year={2022}}"
    >}}
        <a href="#" class="btn-action btn-primary"><i class="fas fa-file-pdf"></i> PDF</a>
        <a href="#" class="btn-action"><i class="fab fa-github"></i> Code</a>
        <button class="btn-action" onclick="toggleBibtex('bib6')"><i class="fas fa-quote-right"></i> BibTeX</button>
        <a href="#" class="btn-action"><i class="fas fa-external-link-alt"></i> arXiv</a>
    {{< /publication_item >}}
    {{< publication_item
        title="Deep Fusion Prior for Plenoptic Super-resolution All-in-focus Imaging"
        year="2022"
        type="journal"
        tags="ai,imaging"
        search="plenoptic super-resolution all-in-focus imaging"
        authors="<span class='author-me'>Yuanjie Gu</span>, Yinghan Guan, Zhibo Xiao, Haoran Dai, Cheng Liu, Shouyu Wang"
        venue="Optical Engineering"
        meta="<span><i class='fas fa-calendar'></i> 2022</span><span><i class='fas fa-book'></i> Opt. Eng.</span><span><i class='fas fa-star'></i> IF: ~1.3</span><span><i class='fas fa-quote-right'></i> Citations: TBD</span>"
        bibtexId="bib8"
        bibtexKey="gu2022deepfusion"
        bibtexContent="@article{gu2022deepfusion, title={Deep Fusion Prior for Plenoptic Super-resolution All-in-focus Imaging}, author={Gu, Yuanjie and Guan, Yinghan and Xiao, Zhibo and Dai, Haoran and Liu, Cheng and Wang, Shouyu}, journal={Optical Engineering}, volume={61}, number={12}, pages={123103}, year={2022}}"
    >}}
        <a href="#" class="btn-action btn-primary"><i class="fas fa-file-pdf"></i> PDF</a>
        <a href="#" class="btn-action"><i class="fab fa-github"></i> Code</a>
        <button class="btn-action" onclick="toggleBibtex('bib8')"><i class="fas fa-quote-right"></i> BibTeX</button>
        <a href="#" class="btn-action"><i class="fas fa-external-link-alt"></i> arXiv</a>
    {{< /publication_item >}}
    {{< publication_item
        title="OpenRefocus: An Open-source Qt-based Tool for Light Field Parallel Refocusing"
        year="2022"
        type="journal"
        tags="software,imaging"
        search="light field refocusing open-source"
        authors="<span class='author-me'>Yuanjie Gu</span>, Miao Yu, Lingyu Ai, Zhilong Jiang, Xiaoliang He, Yan Kong, Shouyu Wang"
        venue="Optical Engineering"
        meta="<span><i class='fas fa-calendar'></i> 2022</span><span><i class='fas fa-book'></i> Opt. Eng.</span><span><i class='fas fa-star'></i> IF: ~1.3</span><span><i class='fas fa-quote-right'></i> Citations: TBD</span>"
        bibtexId="bib9"
        bibtexKey="gu2022openrefocus"
        bibtexContent="@article{gu2022openrefocus, title={OpenRefocus: An Open-source Qt-based Tool for Light Field Parallel Refocusing}, author={Gu, Yuanjie and Yu, Miao and Ai, Lingyu and Jiang, Zhilong and He, Xiaoliang and Kong, Yan and Wang, Shouyu}, journal={Optical Engineering}, volume={61}, number={6}, pages={063108}, year={2022}}"
    >}}
        <a href="#" class="btn-action btn-primary"><i class="fas fa-file-pdf"></i> PDF</a>
        <a href="#" class="btn-action"><i class="fab fa-github"></i> Code</a>
        <button class="btn-action" onclick="toggleBibtex('bib9')"><i class="fas fa-quote-right"></i> BibTeX</button>
        <a href="#" class="btn-action"><i class="fas fa-external-link-alt"></i> arXiv</a>
    {{< /publication_item >}}
    {{< publication_item
        title="Automatic Whole Blood Cell Analysis from Blood Smear using Label-free Multi-modal Imaging with Deep Neural Networks"
        year="2022"
        type="journal"
        tags="ai,medical"
        search="blood cell analysis multi-modal imaging deep learning"
        authors="Chao Chen, <span class='author-me'>Yuanjie Gu</span>, Zhibo Xiao, Hailun Wang, Xiaoliang He, Zhilong Jiang, Yan Kong, Cheng Liu, Liang Xue, Javier Vargas, Shouyu Wang"
        venue="Analytica Chimica Acta"
        meta="<span><i class='fas fa-calendar'></i> 2022</span><span><i class='fas fa-book'></i> Anal. Chim. Acta</span><span><i class='fas fa-star'></i> IF: ~6.2</span><span><i class='fas fa-quote-right'></i> Citations: TBD</span>"
        bibtexId="bib17"
        bibtexKey="chen2022automatic"
        bibtexContent="@article{chen2022automatic, title={Automatic Whole Blood Cell Analysis from Blood Smear using Label-free Multi-modal Imaging with Deep Neural Networks}, author={Chen, Chao and Gu, Yuanjie and Xiao, Zhibo and Wang, Hailun and He, Xiaoliang and Jiang, Zhilong and Kong, Yan and Liu, Cheng and Xue, Liang and Vargas, Javier and Wang, Shouyu}, journal={Analytica Chimica Acta}, volume={1229}, pages={340401}, year={2022}}"
    >}}
        <a href="#" class="btn-action btn-primary"><i class="fas fa-file-pdf"></i> PDF</a>
        <a href="#" class="btn-action"><i class="fab fa-github"></i> Code</a>
        <button class="btn-action" onclick="toggleBibtex('bib17')"><i class="fas fa-quote-right"></i> BibTeX</button>
        <a href="#" class="btn-action"><i class="fas fa-external-link-alt"></i> arXiv</a>
    {{< /publication_item >}}
    <!-- ================================================================================== -->
    <!-- 2021 Papers -->
    <!-- ================================================================================== -->
    {{< publication_item
        title="REPAID: Resolution-enhanced Plenoptic All-in-focus Imaging using Deep Neural Networks"
        year="2021"
        type="journal"
        tags="ai,imaging"
        search="plenoptic all-in-focus imaging deep learning"
        authors="Miao Yu, <span class='author-me'>Yuanjie Gu</span>, Zhilong Jiang, Xiaoliang He, Yan Kong, Cheng Liu, Shouyu Wang"
        venue="Optics Letters"
        meta="<span><i class='fas fa-calendar'></i> 2021</span><span><i class='fas fa-book'></i> Opt. Lett.</span><span><i class='fas fa-star'></i> IF: ~3.6</span><span><i class='fas fa-quote-right'></i> Citations: TBD</span>"
        bibtexId="bib11"
        bibtexKey="yu2021repaid"
        bibtexContent="@article{yu2021repaid, title={REPAID: Resolution-enhanced Plenoptic All-in-focus Imaging using Deep Neural Networks}, author={Yu, Miao and Gu, Yuanjie and Jiang, Zhilong and He, Xiaoliang and Kong, Yan and Liu, Cheng and Wang, Shouyu}, journal={Optics Letters}, volume={46}, number={12}, pages={2896-2899}, year={2021}}"
    >}}
        <a href="#" class="btn-action btn-primary"><i class="fas fa-file-pdf"></i> PDF</a>
        <a href="#" class="btn-action"><i class="fab fa-github"></i> Code</a>
        <button class="btn-action" onclick="toggleBibtex('bib11')"><i class="fas fa-quote-right"></i> BibTeX</button>
        <a href="#" class="btn-action"><i class="fas fa-external-link-alt"></i> arXiv</a>
    {{< /publication_item >}}

</div>

</div>

<!-- 引入 JavaScript -->
{{< publications_js >}}