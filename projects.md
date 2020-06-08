---
title: Projects | Kian Faizi
layout: default
---
<header>
    <nav>
        <ul>
            <li><a href="/">Kian Faizi</a></li>
            <li><a href="/contact.html">Contact</a></li>
            <li><a href="/blog.html">Blog</a></li>
            <li><a href="/cv.html">CV</a></li>
            <li><a href="/projects.html" class="active">Projects</a></li>
        </ul>
    </nav>
</header>

# My Projects

My interests lie in **studying complex biological systems using quantitative and computational approaches**. I want to leverage this knowledge to engineer synthetic organisms to advance the health of people and the planet.

## Summary of past work
Currently, I'm a lab technician in [Professor Wolfgang Busch’s group] at the Salk Institute. We study the genetics underlying root growth and root-environment interactions in plants, with a focus on the model organism _Arabidopsis thaliana_. A major goal of this research is facilitating crop engineering efforts to [fight climate change]. To aid root phenotyping tasks, I developed an image analysis tool. I'm also working on the network-based identification of functional homologs of genes driving root depth, based on coexpression analysis of single-cell RNA-seq data.

Previously, I volunteered in the [lab of Dr. Patrick Hsu], where I helped develop tools for RNA editing using CRISPR-Cas13d. I wrote a pipeline for discovering new orthologs of Cas13d, and helped conduct a pooled transcriptome-wide screen to investigate guide RNA efficiency.

[Professor Wolfgang Busch’s group]: https://busch.salk.edu/ "Busch Lab homepage"
{:target="_blank" rel="noreferrer noopener"}

[fight climate change]: https://www.salk.edu/science/power-of-plants/ "Harnessing Plants Initiative"
{:target="_blank" rel="noreferrer noopener"}

[lab of Dr. Patrick Hsu]: http://patrickhsulab.org/ "Hsu Lab homepage"
{:target="_blank" rel="noreferrer noopener"}

## Software
Please note: all project names are horrible temporary placeholders.

<div class="project-wrapper">
<div class="project-info" markdown="1">
**rootmarker** is a Python GUI for manually segmenting 2D scans of plant roots. Users point and click to place nodes, creating a skeletonized graph that describes the root system architecture. Includes support for annotating time-series GIFs. [Repo]
</div>
<div class="project-media">
<img class="project-img" src="/assets/rootmarker.png">
</div>
</div>

<div class="project-wrapper">
<div class="project-info" markdown="1">
**CRISPRminer** is a bioinformatics pipeline for mining large-scale metagenomic sequence data to discover new Cas proteins. Prokaryotic genomes and metagenomes are searched for new orthologs of known (input) effectors with <span class="inline-code">TBLASTN</span>. Putative hits are screened for arrays using <span class="inline-code">CRISPRFinder</span>, and filtered by size, distance, and sequence identity.
</div>
<div class="project-media">
<img class="project-img" src="/assets/crisprminer.png">
</div>
</div>


[Repo]:https://github.com/kfaizi/test-roots
{:target="_blank" rel="noreferrer noopener"}
