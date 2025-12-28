---
title: "Publications"
description: "Selected peer-reviewed journals and conference proceedings."
layout: "simple"
fullWidth: true 
showDate: false
---

<style>
.publication-card {
    border: 1px solid #e5e5e5;
    border-radius: 8px;
    padding: 20px;
    margin-bottom: 20px;
    transition: all 0.3s ease;
    background-color: white;
}

.dark .publication-card {
    border-color: #374151;
    background-color: #1f2937;
}

.publication-card:hover {
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    transform: translateY(-2px);
}

.dark .publication-card:hover {
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.3);
}

.publication-header {
    font-size: 1.25rem;
    font-weight: 600;
    margin-bottom: 10px;
    color: #111827;
}

.dark .publication-header {
    color: #f3f4f6;
}

.publication-details {
    margin-bottom: 15px;
    color: #4b5563;
    font-size: 0.875rem;
}

.dark .publication-details {
    color: #d1d5db;
}

.publication-details em {
    font-style: normal;
    font-weight: 600;
    color: #374151;
}

.dark .publication-details em {
    color: #9ca3af;
}

.publication-links {
    display: flex;
    gap: 10px;
    flex-wrap: wrap;
}

.year-badge {
    display: inline-block;
    background-color: #3b82f6;
    color: white;
    padding: 2px 8px;
    border-radius: 4px;
    font-size: 0.75rem;
    font-weight: 600;
    margin-right: 8px;
}

.type-badge {
    display: inline-block;
    background-color: #10b981;
    color: white;
    padding: 2px 8px;
    border-radius: 4px;
    font-size: 0.75rem;
    font-weight: 600;
    margin-right: 8px;
}

.publication-stats {
    text-align: center;
    padding: 20px;
    background-color: #f9fafb;
    border-radius: 8px;
    margin-bottom: 30px;
}

.dark .publication-stats {
    background-color: #374151;
}

.stat-number {
    font-size: 2rem;
    font-weight: 700;
    color: #3b82f6;
}

.dark .stat-number {
    color: #60a5fa;
}

.stat-label {
    font-size: 0.875rem;
    color: #6b7280;
}

.dark .stat-label {
    color: #9ca3af;
}

.filter-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
    margin-bottom: 20px;
}

.filter-tag {
    padding: 4px 12px;
    border-radius: 16px;
    font-size: 0.875rem;
    cursor: pointer;
    transition: all 0.2s ease;
    border: 1px solid #e5e7eb;
}

.filter-tag:hover {
    background-color: #f3f4f6;
}

.dark .filter-tag:hover {
    background-color: #374151;
}

.filter-tag.active {
    background-color: #3b82f6;
    color: white;
    border-color: #3b82f6;
}

.author-highlight {
    font-weight: 600;
    color: #111827;
    text-decoration: underline;
    text-decoration-color: #3b82f6;
    text-underline-offset: 2px;
}

.dark .author-highlight {
    color: #f3f4f6;
    text-decoration-color: #60a5fa;
}

.toc {
    background-color: #f9fafb;
    border-radius: 8px;
    padding: 20px;
    margin-bottom: 30px;
}

.dark .toc {
    background-color: #374151;
}

.toc h3 {
    margin-top: 0;
    margin-bottom: 10px;
}

.toc ul {
    margin: 0;
    padding-left: 20px;
}

.toc li {
    margin-bottom: 5px;
}
</style>

<!-- 出版物统计 -->
<div class="publication-stats">
    <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
        <div>
            <div class="stat-number">15</div>
            <div class="stat-label">Total Papers</div>
        </div>
        <div>
            <div class="stat-number">10</div>
            <div class="stat-label">Journal Articles</div>
        </div>
        <div>
            <div class="stat-number">5</div>
            <div class="stat-label">Conference Papers</div>
        </div>
        <div>
            <div class="stat-number">3</div>
            <div class="stat-label">First Author</div>
        </div>
    </div>
</div>

<!-- 目录 -->
<div class="toc">
    <h3 class="text-lg font-semibold mb-3">Table of Contents</h3>
    <ul>
        <li><a href="#journal-articles" class="text-blue-600 hover:underline">Journal Articles</a></li>
        <li><a href="#conference-proceedings" class="text-blue-600 hover:underline">Conference Proceedings</a></li>
        <li><a href="#preprints" class="text-blue-600 hover:underline">Preprints</a></li>
        <li><a href="#patents" class="text-blue-600 hover:underline">Patents</a></li>
    </ul>
</div>

<!-- 过滤器标签 -->
<div class="filter-tags">
    <span class="filter-tag active">All</span>
    <span class="filter-tag">2024</span>
    <span class="filter-tag">2023</span>
    <span class="filter-tag">First Author</span>
    <span class="filter-tag">AI/ML</span>
    <span class="filter-tag">Computer Vision</span>
    <span class="filter-tag">Systems</span>
</div>

<h2 id="journal-articles" class="text-2xl font-bold mt-8 mb-6 pb-2 border-b">Journal Articles</h2>

<div class="publication-card">
    <div class="publication-header">
        <span class="year-badge">2024</span>
        <span class="type-badge">Journal</span>
        Towards Scalable Visual Representation Learning with Masked Generative Pretraining
    </div>
    <div class="publication-details">
        <em>Authors:</em> <span class="author-highlight">Your Name*</span>, Jane Smith, John Doe, Robert Brown<br>
        <em>Journal:</em> IEEE Transactions on Pattern Analysis and Machine Intelligence (TPAMI)<br>
        <em>Status:</em> In Press<br>
        <em>Impact Factor:</em> 24.314<br>
        <em>Abstract:</em> This paper introduces a novel masked generative pretraining framework for learning scalable visual representations. Our method achieves state-of-the-art performance on multiple benchmarks while requiring 40% less training time compared to previous approaches.
    </div>
    <div class="publication-links">
        <a href="#" class="px-4 py-2 bg-blue-600 text-white text-sm rounded-md hover:bg-blue-700 transition">PDF</a>
        <a href="#" class="px-4 py-2 bg-gray-200 text-gray-800 text-sm rounded-md hover:bg-gray-300 transition dark:bg-gray-700 dark:text-gray-200">arXiv</a>
        <a href="#" class="px-4 py-2 bg-gray-800 text-white text-sm rounded-md hover:bg-gray-900 transition">Code</a>
        <a href="#" class="px-4 py-2 bg-green-600 text-white text-sm rounded-md hover:bg-green-700 transition">BibTeX</a>
    </div>
</div>

<div class="publication-card">
    <div class="publication-header">
        <span class="year-badge">2023</span>
        <span class="type-badge">Journal</span>
        Efficient Federated Learning for Edge Computing with Adaptive Client Selection
    </div>
    <div class="publication-details">
        <em>Authors:</em> <span class="author-highlight">Your Name*</span>, Alice Johnson, Bob Wilson<br>
        <em>Journal:</em> ACM Transactions on Intelligent Systems and Technology (TIST)<br>
        <em>Volume:</em> 14, Issue 3<br>
        <em>Pages:</em> 1-24<br>
        <em>DOI:</em> <a href="https://doi.org/10.1145/3582425" class="text-blue-600 hover:underline">10.1145/3582425</a><br>
        <em>Impact Factor:</em> 6.143<br>
        <em>Abstract:</em> We propose an adaptive client selection strategy for federated learning in edge computing environments, reducing communication overhead by 60% while maintaining model accuracy.
    </div>
    <div class="publication-links">
        <a href="#" class="px-4 py-2 bg-blue-600 text-white text-sm rounded-md hover:bg-blue-700 transition">PDF</a>
        <a href="#" class="px-4 py-2 bg-gray-200 text-gray-800 text-sm rounded-md hover:bg-gray-300 transition dark:bg-gray-700 dark:text-gray-200">DOI</a>
        <a href="#" class="px-4 py-2 bg-gray-800 text-white text-sm rounded-md hover:bg-gray-900 transition">Code</a>
    </div>
</div>

<h2 id="conference-proceedings" class="text-2xl font-bold mt-12 mb-6 pb-2 border-b">Conference Proceedings</h2>

<div class="publication-card">
    <div class="publication-header">
        <span class="year-badge">2024</span>
        <span class="type-badge" style="background-color: #8b5cf6;">Conference</span>
        Dynamic Neural Radiance Fields for Real-time View Synthesis
    </div>
    <div class="publication-details">
        <em>Authors:</em> <span class="author-highlight">Your Name*</span>, Carol Davis, Michael Lee<br>
        <em>Conference:</em> IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)<br>
        <em>Location:</em> Seattle, WA, USA<br>
        <em>Acceptance Rate:</em> 25.8%<br>
        <em>Abstract:</em> We present a dynamic neural radiance field method that achieves real-time novel view synthesis of dynamic scenes, outperforming previous methods by 2.5× in rendering speed.
    </div>
    <div class="publication-links">
        <a href="#" class="px-4 py-2 bg-blue-600 text-white text-sm rounded-md hover:bg-blue-700 transition">PDF</a>
        <a href="#" class="px-4 py-2 bg-purple-600 text-white text-sm rounded-md hover:bg-purple-700 transition">Project Page</a>
        <a href="#" class="px-4 py-2 bg-gray-800 text-white text-sm rounded-md hover:bg-gray-900 transition">Code</a>
        <a href="#" class="px-4 py-2 bg-red-600 text-white text-sm rounded-md hover:bg-red-700 transition">Video</a>
    </div>
</div>

<div class="publication-card">
    <div class="publication-header">
        <span class="year-badge">2023</span>
        <span class="type-badge" style="background-color: #8b5cf6;">Conference</span>
        Multi-modal Fusion for Robust 3D Object Detection in Autonomous Driving
    </div>
    <div class="publication-details">
        <em>Authors:</em> David Chen, <span class="author-highlight">Your Name</span>, Sarah Williams<br>
        <em>Conference:</em> International Conference on Computer Vision (ICCV)<br>
        <em>Location:</em> Paris, France<br>
        <em>Pages:</em> 12345-12356<br>
        <em>Abstract:</em> This work proposes a novel multi-modal fusion network that combines LiDAR and camera data for robust 3D object detection, achieving state-of-the-art results on nuScenes dataset.
    </div>
    <div class="publication-links">
        <a href="#" class="px-4 py-2 bg-blue-600 text-white text-sm rounded-md hover:bg-blue-700 transition">PDF</a>
        <a href="#" class="px-4 py-2 bg-gray-800 text-white text-sm rounded-md hover:bg-gray-900 transition">Code</a>
        <a href="#" class="px-4 py-2 bg-green-600 text-white text-sm rounded-md hover:bg-green-700 transition">Dataset</a>
    </div>
</div>

<h2 id="preprints" class="text-2xl font-bold mt-12 mb-6 pb-2 border-b">Preprints</h2>

<div class="publication-card">
    <div class="publication-header">
        <span class="year-badge">2024</span>
        <span class="type-badge" style="background-color: #f59e0b;">Preprint</span>
        Towards Generalizable Robot Manipulation with Large Vision-Language Models
    </div>
    <div class="publication-details">
        <em>Authors:</em> <span class="author-highlight">Your Name*</span>, Thomas Anderson, Lisa Wong<br>
        <em>Repository:</em> arXiv<br>
        <em>Preprint:</em> <a href="https://arxiv.org/abs/2401.12345" class="text-blue-600 hover:underline">arXiv:2401.12345</a><br>
        <em>Submitted to:</em> Robotics: Science and Systems (RSS)<br>
        <em>Abstract:</em> We investigate the use of large vision-language models for generalizable robot manipulation tasks, demonstrating zero-shot transfer to unseen objects and environments.
    </div>
    <div class="publication-links">
        <a href="#" class="px-4 py-2 bg-orange-600 text-white text-sm rounded-md hover:bg-orange-700 transition">arXiv</a>
        <a href="#" class="px-4 py-2 bg-gray-800 text-white text-sm rounded-md hover:bg-gray-900 transition">Code</a>
        <a href="#" class="px-4 py-2 bg-red-600 text-white text-sm rounded-md hover:bg-red-700 transition">Demo</a>
    </div>
</div>

<h2 id="patents" class="text-2xl font-bold mt-12 mb-6 pb-2 border-b">Patents</h2>

<div class="publication-card">
    <div class="publication-header">
        <span class="year-badge">2023</span>
        <span class="type-badge" style="background-color: #ec4899;">Patent</span>
        System and Method for Real-time Anomaly Detection in Industrial IoT Networks
    </div>
    <div class="publication-details">
        <em>Inventors:</em> <span class="author-highlight">Your Name</span>, Robert Johnson, Maria Garcia<br>
        <em>Patent Number:</em> US 11,654,321 B2<br>
        <em>Filing Date:</em> March 15, 2023<br>
        <em>Issue Date:</em> October 10, 2023<br>
        <em>Assignee:</em> Tech Innovations Inc.<br>
        <em>Abstract:</em> A system for real-time anomaly detection in industrial IoT networks using ensemble learning techniques with adaptive thresholding.
    </div>
    <div class="publication-links">
        <a href="#" class="px-4 py-2 bg-pink-600 text-white text-sm rounded-md hover:bg-pink-700 transition">Patent</a>
        <a href="#" class="px-4 py-2 bg-gray-200 text-gray-800 text-sm rounded-md hover:bg-gray-300 transition dark:bg-gray-700 dark:text-gray-200">Google Patents</a>
    </div>
</div>

<hr class="my-12">

<div class="text-center text-gray-600 dark:text-gray-400 text-sm">
    <p><strong>Note:</strong> * indicates corresponding author</p>
    <p class="mt-2">For a complete list of publications, please visit my 
        <a href="https://scholar.google.com" class="text-blue-600 hover:underline">Google Scholar</a> or 
        <a href="https://orcid.org" class="text-blue-600 hover:underline">ORCID</a> profile.
    </p>
</div>