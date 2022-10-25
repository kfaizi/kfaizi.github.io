---
layout: default
---
<header>
    <nav>
        <ul>
            <li><a href="/" class="active">Home</a></li>
            <li><a href="/blog.html">Blog</a></li>
            <li><a href="/assets/kian-faizi-cv.pdf">CV</a></li>
        </ul>
    </nav>
</header>

<!-- new stuff -->
<!-- Master table -->
<table class="index">
  <tbody>
    <tr style="padding:0px">
      <td style="padding:0px">

        <!-- Introduction -->
        <table class="index" id="intro-table">
          <tbody>
            <tr style="padding:0px">
              <td style="width:63%;vertical-align:middle;">
                <p style="text-align:center">
                  <h1 style="text-align: center;">
                    <span class="tooltip">Kian Faizi<span class="tooltip-text">/kiɑn fɑɪzi/</span></span>
                  </h1>
                </p>
              </td>
              <td>
              </td>
            </tr>
            <tr style="padding:0px">
              <td style="width:63%;vertical-align:top">
                <p>
                  Hi, I'm Kian! I'm interested in how life works — and how we can engineer it to make the world a better place.
                </p>                  
                <p>
                  I'm a PhD student at Caltech in the systems biology program. This summer, I was on sabbatical at Harvard as an inaugural <a href="https://www.newscience.org" target="_blank" rel="noreferrer noopener">New Science</a> summer fellow.
                </p>
                <p>
                  <highlight>If it sounds like our interests align, <a href="mailto:kian@caltech.edu">say hi</a>!</highlight> I'm always excited to talk science with new people. You can also find me on <a href="https://www.twitter.com/kianfaizi/" target="_blank" rel="noreferrer noopener">Twitter</a> and <a href="https://www.github.com/kfaizi/" target="_blank" rel="noreferrer noopener">GitHub</a>.
                </p>
              </td>
              <td style="max-width:30%;vertical-align:text-top;padding-left:3%">
                <a href="/assets/images/rainier-headshot.jpg" id="headshot"><img alt="headshot" title="it's me!" src="/assets/images/cropped-rainier-headshot.png"></a>
              </td>
            </tr>
          </tbody>
        </table>

        <!-- newsfeed -->
        <!-- <h2>Newsfeed</h2>
        <p>Placeholder text</p>
        <table>
          <thead>
            <tr>
              <th>date</th>
              <th>description</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>(2022-07-07)</td>
              <td>placeholder text!</td>
            </tr>
          </tbody>
        </table> 
        <br>-->



        <!-- Blog -->
        <h2>Blog</h2>
        <table class="index">
          <tbody>
            <tr>
              <td>
                <p>
                  <a href="/blog.html">Sometimes I write</a> about science, programming, and anything else I'm currently curious about. Check out my most recent posts below:
                </p>

                <ul class="posts">
                  {% for post in site.posts limit:5 %}
                      <li>
                      {% if post.external_url %}
                          <a href="{{ post.external_url }}">{{ post.title }} ↗</a> (published at {{post.external_host}}) <span id="post-date">({{ post.date | date: "%-m/%-d/%y" }})</span>
                      {% else %}
                          <a href="{{ post.url }}">{{ post.title }}</a> <span id="post-date">({{ post.date | date: "%-m/%-d/%y" }})</span>
                      {% endif %}    
                      </li>
                  {% endfor %}
                </ul>

                <!-- <ul>
                  {% for post in site.posts limit:5 %}
                    <li>
                      <a href="{{ post.url }}">{{ post.title }}</a> <span id="post-date">({{ post.date | date: "%-Y-%m-%d" }})</span>
                    </li>
                  {% endfor %}
                </ul> -->

              </td>
            </tr>
          </tbody>
        </table>

        <!-- Research interests -->
        <h2>Research</h2>
        <table class="index">
          <tbody>
            <tr>
              <td>
                <p>
                  I enjoy thinking about how mathematical models and physical laws can describe (and predict!) cellular behavior. I'm fascinated by developmental plasticity and self-organization in biological systems.
                </p>
                <p>
                  I did my undergrad at UCSD studying molecular biology and math. While there, I was a tech in <a href="https://www.busch.salk.edu/" target="_blank" rel="noreferrer noopener">Dr. Wolfgang Busch's</a> plant genetics group at the Salk Institute, where I studied root-environment interactions in <i>Arabidopsis thaliana</i> using quantitative and computational methods. Before that, I worked in <a href="http://www.patrickhsulab.org/" target="_blank" rel="noreferrer noopener">Dr. Patrick Hsu's</a> lab, where I helped develop CRISPR-Cas13d for programmable RNA editing. See <a href="/assets/kian-faizi-cv.pdf">my CV</a> for more details, or read about some of my projects below:
                </p>
              </td>
            </tr>
          </tbody>
        </table>

        <p>
        </p>

        <!-- Publications and projects -->
        <table class="index">
          <tbody>

            <!-- pub -->
            <!-- <tr>
              <td class="project-media">
                <img class="project-img" src="/assets/images/screen.jpg" alt="alt" title="title">
              </td>
              <td class="project-info">
                <span class="project-title">Towards a free-living chloroplast</span>
                <br>
                <highlight>Kian Faizi</highlight>
                <br>
                <input type="checkbox" id="trigger3">
                [<label for="trigger3"><a id="fakelink">abstract</a></label>]
                <span id="box">
                  Abstract here.
                </span> /
                [<a href="/" target="_blank" rel="noreferrer noopener">proposal</a>] /
                [<a href="https://newscience.org/2022-summer-fellows/" target="_blank" rel="noreferrer noopener">press release</a>]
                <p></p>
                <p>
                  Blurb.
                </p>
              </td>
            </tr> -->


            <!-- pub -->
            <tr>
              <td class="project-media">
                <img class="project-img" src="/assets/images/catastrophe.jpg" alt="catastrophe" title="things fall apart">
              </td>
              <td class="project-info">
                <span class="project-title">Modeling Microtubule Catastrophe</span>
                <br>
                <highlight>Kian Faizi</highlight>, David Jin, <a href="https://scholar.google.com/citations?view_op=list_works&hl=en&user=44KjzP0AAAAJ" target="_blank" rel="noreferrer noopener">James Mullahoo</a>, Ziyan Wu
                <br>
                [<a href="https://www.kianfaizi.com/catastrophe/index.html" target="_blank" rel="noreferrer noopener">website</a>] /
                [<a href="https://github.com/kfaizi/catastrophe" title="catastrophe on GitHub" target="_blank" rel="noreferrer noopener">code</a>]
                <p></p>
                <p>
                  I built a website showcasing my team's analysis of the dynamics of microtubule growth, based on <a href="https://gchure.github.io" target="_blank" rel="noreferrer noopener">Griffin Chure's</a> template for reproducible research. Class project for <a href="https://bebi103a.github.io" target="_blank" rel="noreferrer noopener">BE/Bi 103a</a>.
                </p>
              </td>
            </tr>


            <!-- pub -->
            <tr>
              <td class="project-media">
                <img class="project-img" src="/assets/images/screen.jpg" alt="screen" title="there was a lot of TC work">
              </td>
              <td class="project-info">
                <span class="project-title">Deep learning and CRISPR-Cas13d ortholog discovery for optimized RNA targeting</span>
                <br>
                <a href="https://twitter.com/JingyiWei4" target="_blank" rel="noreferrer noopener">Jingyi Wei</a>, <a href="https://www.linkedin.com/in/peter-lotfy-ba045684/" target="_blank" rel="noreferrer noopener">Peter Lotfy</a>, <highlight>Kian Faizi</highlight>, <a href="https://twitter.com/EleanorWang" target="_blank" rel="noreferrer noopener">Eleanor Wang</a>, <a href="https://www.linkedin.com/in/slabodkin/" target="_blank" rel="noreferrer noopener">Hannah Slabodkin</a>, Emily Kinnaman, <a href="https://www.linkedin.com/in/sita-c-990a40171/" target="_blank" rel="noreferrer noopener">Sita Chandrasekaran</a>, Hugo Kitano, <a href="https://scholar.google.com/citations?user=hUi_OqkAAAAJ" target="_blank" rel="noreferrer noopener">Matthew G. Durrant</a>, <a href="https://scholar.google.com/citations?user=0vx-lmkAAAAJ&hl=en&oi=ao" target="_blank" rel="noreferrer noopener">Connor V. Duffy</a>, <a href="https://bioeng.berkeley.edu/faculty/patrick-hsu" target="_blank" rel="noreferrer noopener">Patrick D. Hsu</a>, <a href="https://biochemistry.stanford.edu/silvana-konermann" target="_blank" rel="noreferrer noopener">Silvana Konermann</a>
                <br>
                <i>bioRxiv.</i> (2021)
                <br>
                <input type="checkbox" id="trigger2">
                [<label for="trigger2"><a id="fakelink">abstract</a></label>]
                <span id="box">
                  Transcriptome engineering technologies that can effectively and precisely perturb mammalian RNAs are needed to accelerate biological discovery and RNA therapeutics. However, the broad utility of programmable CRISPR-Cas13 ribonucleases has been hampered by an incomplete understanding of the design rules governing guide RNA activity as well as cellular toxicity resulting from off-target or collateral RNA cleavage. Here, we sought to characterize and develop Cas13d systems for efficient and specific RNA knockdown with low cellular toxicity in human cells. We first quantified the performance of over 127,000 RfxCas13d (CasRx) guide RNAs in the largest-scale screen to date and systematically evaluated three linear, two ensemble, and two deep learning models to build a guide efficiency prediction algorithm validated across multiple human cell types in orthogonal secondary screens (<a href="http://RNAtargeting.org">http://RNAtargeting.org</a>). Deep learning model interpretation revealed specific sequence motifs at spacer position 15-24 along with favored secondary features for highly efficient guides. We next identified 46 novel Cas13d orthologs through metagenomic mining for activity screening, discovering that the metagenome-derived DjCas13d ortholog achieves low cellular toxicity and high transcriptome-wide specificity when deployed against high abundance transcripts or in sensitive cell types, including hESCs. Finally, our Cas13d guide efficiency model successfully generalized to DjCas13d, highlighting the utility of a comprehensive approach combining machine learning with ortholog discovery to advance RNA targeting in human cells.
                </span> /
                [<a href="https://doi.org/10.1101/2021.09.14.460134" target="_blank" rel="noreferrer noopener">preprint</a>]
                <p></p>
                <p>
                  I helped conduct a 127,000-guide CRISPR-Cas13d screen to identify guide RNA design rules and optimize transcriptome editing efficiency.
                </p>
              </td>
            </tr>
            
            <!-- pub -->
            <tr>
              <td class="project-media">
                <img class="project-img" src="/assets/images/p3d.jpg" alt="p3d" title="skeletonization algorithm goes brrrr">
              </td>
              <td class="project-info">
                <span class="project-title">Branch-Pipe: Improving graph skeletonization around branch points in 3D point clouds</span>
                <br>
                <a href="https://www.linkedin.com/in/illiaziamtsov/" target="_blank" rel="noreferrer noopener">Illia Ziamtsov</a>, <highlight>Kian Faizi</highlight>, <a href="https://www.cshl.edu/research/faculty-staff/saket-navlakha/" target="_blank" rel="noreferrer noopener">Saket Navlakha</a>
                <br>
                <i>Remote Sensing (open access).</i> (2021)
                <br>
                <input type="checkbox" id="trigger1">
                [<label for="trigger1"><a id="fakelink">abstract</a></label>]
                <span id="box">
                  Modern plant phenotyping requires tools that are robust to noise and missing data, while being able to efficiently process large numbers of plants. In this manuscript, we studied skeletonization of plant architectures from 3D point clouds, which is critical for many downstream tasks, including analyses of plant shape, morphology, and branching angles. Specifically, we developed an algorithm to improve skeletonization at branch points (forks) by leveraging geometric properties of cylinders around branch points. We tested this algorithm on a diverse set of high-resolution 3D point clouds of tomato and tobacco plants, grown in five environments and across multiple developmental timepoints. Compared to existing methods for 3D skeletonization, our method efficiently and more accurately estimated branching angles, even in areas with noisy, missing, or non-uniformly sampled data. Our method is also applicable to inorganic datasets, such as scans of industrial pipes or urban scenes containing networks of complex cylindrical shapes.
                </span> /
                [<a href="https://doi.org/10.3390/rs13193802" target="_blank" rel="noreferrer noopener">paper</a>] /
                [<a href="https://twitter.com/kianfaizi/status/1441069414837731343?s=20" target="_blank" rel="noreferrer noopener">thread</a>]
                <p></p>
                <p>
                  I assisted in the development of a software package for plant phenotyping, with a focus on accurate skeleton graph extraction from noisy 3D point clouds.
                </p>
              </td>
            </tr>

            <!-- pub -->
            <tr>
              <td class="project-media">
                <img class="project-img" src="/assets/images/rootmarker.png" alt="ariadne" title="n paths diverged on an agar plate...">
              </td>
              <td class="project-info">
                <span class="project-title">Network Design Principles in the <i>Arabidopsis</i> Root System</span>
                <br>
                <highlight>Kian Faizi</highlight>, <a href="https://scholar.google.com/citations?user=heUMphcAAAAJ&hl=en&oi=ao" target="_blank" rel="noreferrer noopener">Matthieu Platre</a>, <a href="https://www.arjun-chandrasekhar-teaching.com" target="_blank" rel="noreferrer noopener">Arjun Chandrasekhar</a>, <a href="https://www.cshl.edu/research/faculty-staff/saket-navlakha/" target="_blank" rel="noreferrer noopener">Saket Navlakha</a>, <a href="https://www.salk.edu/scientist/wolfgang-busch/" target="_blank" rel="noreferrer noopener">Wolfgang Busch</a>
                <br>
                <i>manuscript in preparation</i>
                <br>
                <!-- <input type="checkbox" id="trigger3">
                <label for="trigger3"><a id="fakelink">abstract</a></label>
                <span id="box">
                  <b>rootmarker</b> is a Python GUI for manually segmenting 2D scans of plant roots. Users point and click to place nodes, creating a skeletonized graph that describes the root system architecture. Includes support for annotating time-series GIFs.
                </span> / -->
                [<a href="https://github.com/kfaizi/ariadne" title="ariadne on GitHub" target="_blank" rel="noreferrer noopener">code</a>]
                <p></p>
                <p>
                  I developed Ariadne, a time-series image segmentation tool for root phenotyping, and used it to measure Pareto-optimal trade-offs in root growth.
                </p>
              </td>
            </tr>

            <!-- pub -->
            <tr>
              <td class="project-media">
                <img class="project-img" src="/assets/images/coexpression.png" alt="coexpression" title="making cytoscape work in jupyter is weirdly hard">
              </td>
              <td class="project-info">
                <span class="project-title">Predicting Functional Homologs from Single-Cell Co-expression Networks</span>
                <br>
                [<a href="https://github.com/kfaizi/coexpression-analysis" title="coexpression-analysis on GitHub" target="_blank" rel="noreferrer noopener">code</a>]
                <p></p>
                <p>
                  I built a basic workflow for predicting functional homologs of genes driving plant root growth, via co-expression network analysis of single-cell RNA-seq data.
                </p>
              </td>
            </tr>

            <!-- pub -->
            <tr>
              <td class="project-media">
                <img class="project-img" src="/assets/images/wiring.png" alt="wiring" title="you may think this is oversimplified. you'd be right">
              </td>
              <td class="project-info">
                <span class="project-title">A Boolean Network Model of the Bacterial <i>lac</i> Operon</span>
                <br>
                [<a href="https://github.com/kfaizi/boolean-lac" title="boolean-lac on GitHub" target="_blank" rel="noreferrer noopener">code</a>]
                <p></p>
                <p>
                  I programmed a toy model of the <i>lac</i> operon as an asynchronous Boolean network, and simulated gene knockout and overexpression experiments. Class project for <a href="https://ccom.ucsd.edu/~acloninger/111A_F20/teachingMath111A.html" target="_blank" rel="noreferrer noopener">MATH 111A</a>.
                </p>
              </td>
            </tr>

            <!-- pub -->
            <tr>
              <td class="project-media">
                <img class="project-img" src="/assets/images/crisprminer.png" alt="crisprminer" title="pretty phylogenetic classification of the variants I found">
              </td>
              <td class="project-info">
                <span class="project-title">Metagenomic Discovery of Novel Type VI-D CRISPR Effectors</span>
                <br>
                <highlight>Kian Faizi</highlight>, <a href="https://biochemistry.stanford.edu/silvana-konermann" target="_blank" rel="noreferrer noopener">Silvana Konermann</a>, <a href="https://bioeng.berkeley.edu/faculty/patrick-hsu" target="_blank" rel="noreferrer noopener">Patrick Hsu</a>
                <br>
                [<a href="/assets/kian-faizi-srs-2019.pdf" title="srs-2019" target="_blank" rel="noreferrer noopener">poster</a>] /
                [<a href="https://github.com/kfaizi/CRISPR-search" title="CRISPR-search on GitHub" target="_blank" rel="noreferrer noopener">code</a>]
                <p></p>
                <p>
                  I wrote a Python pipeline to mine new orthologs of CRISPR-Cas13d from publicly available metagenomic sequence data at terabyte scale.
                </p>
              </td>
            </tr>
          </tbody>
        </table>

        <!-- classes -->
        <h2>Teaching</h2>
        <table class="index">
          <tbody>
            <tr>
              <td class="project-media">
                <img class="project-img" src="/assets/images/sisyphus-titian.jpg" title="one must imagine teaching assistants happy" alt="love">
              </td>
              <td class="project-info">
                <p>
                  Helping people learn is one of my favorite things in the world. In the future, I'd like to compile a list of tools and resources that have helped me get better at doing it. For now, here's a list of classes I've helped teach, as well as any formal feedback I've received:
                </p>
                <p>
                  <i>Note: Caltech doesn't provide a nice way to collate instructor reviews, so I've just copied over any comments I received in plaintext.</i>
                </p>

                <p></p>

                <span class="project-title">Bi 1: Principles of Biology</span>, Caltech, spring 2022
                <br>
                [<a href="/bi1-22-feedback.html" rel="noreferrer noopener">student evaluations</a>]
                
                <p></p>

                <span class="project-title"><a href="https://www.ucsd.edu/catalog/courses/BIOL.html#bicd102" target="_blank" rel="noreferrer noopener">BICD 102: Genetic Inquiry</a></span>, UCSD, fall 2020
                <br>
                [<a href="/assets/Faizi_Kian_Student_IA_Evaluation_BICD_102_FA20.pdf" target="_blank" rel="noreferrer noopener">student evaluations</a>] / [<a href="/assets/Faizi_Kian_Instructor_IA_Evaluation_BICD_102_FA20.pdf" target="_blank" rel="noreferrer noopener">professor's evaluation</a>]
              </td>
            </tr>

          </tbody>
        </table>


        <!-- Acknowledgements -->
        <h2>Acknowledgements</h2>
        <p>
          My homepage layout is inspired by <a href="https://jonbarron.info" target="_blank" rel="noreferrer noopener">this guy</a>.
        </p>


      </td>
    </tr>
  </tbody>
</table>


