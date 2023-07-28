---
layout: default
---
<header>
    <nav>
        <ul>
            <li><a href="/" class="active">home</a></li>
            <li><a href="/blog.html">blog</a></li>
            <li><a href="/assets/kian-faizi-cv.pdf">cv</a></li>
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
                    <span class="tooltip">kian faizi<span class="tooltip-text">/kiɑn fɑɪzi/</span></span>
                  </h1>
                </p>
              </td>
              <td>
              </td>
            </tr>
            <tr style="padding:0px">
              <td style="width:63%;vertical-align:top">
                <p>
                  hi, i'm kian! i'm interested in how life works — and how we can engineer it to make the world a better place.
                </p>                  
                <p>
                  i'm a phd student at caltech in the systems biology program. i was briefly on sabbatical at harvard as an inaugural <a href="https://www.newscience.org" target="_blank" rel="noreferrer noopener">new science</a> summer fellow.
                </p>
                <p>
                  <highlight>if it sounds like our interests align, <a href="mailto:kian@caltech.edu">say hi</a>!</highlight> i'm always excited to talk science with new people. you can also find me on <a href="https://www.twitter.com/kianfaizi/" target="_blank" rel="noreferrer noopener">twitter</a> and <a href="https://www.github.com/kfaizi/" target="_blank" rel="noreferrer noopener">github</a>.
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



        <!-- blog -->
        <h2>blog</h2>
        <table class="index">
          <tbody>
            <tr>
              <td>
                <p>
                  <a href="/blog.html">somtimes i write</a> about science, programming, and anything else i'm currently curious about. check out my most recent posts below:
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
        <h2>research</h2>
        <table class="index">
          <tbody>
            <tr>
              <td>
                <p>
                  i enjoy thinking about how mathematical models and physical laws can describe (and predict!) cellular behavior. i'm fascinated by developmental plasticity and self-organization in biological systems.
                </p>
                <p>
                  i did my undergrad at uc san diego, where i studied molecular biology and math. while there, i was a tech in <a href="https://www.busch.salk.edu/" target="_blank" rel="noreferrer noopener">dr. wolfgang busch's</a> plant genetics group at the salk institute, where i used computer vision to study how roots explore new environments. before that, i worked in <a href="http://www.patrickhsulab.org/" target="_blank" rel="noreferrer noopener">dr. patrick hsu's</a> lab, where i helped develop CRISPR-Cas13d for programmable RNA editing.
                </p>
                <p>
                  for more details, you can <a href="/assets/kian-faizi-cv.pdf">see my cv</a> or read about some of my recent projects:
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
            <!-- <tr>
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
            </tr> -->


            <!-- pub -->
            <tr>
              <td class="project-media">
                <img class="project-img" src="/assets/images/screen.jpg" alt="screen" title="there was a lot of TC work">
              </td>
              <td class="project-info">
                <span class="project-title">Deep learning and CRISPR-Cas13d ortholog discovery for optimized RNA targeting</span>
                <br>
                <a href="https://twitter.com/JingyiWei4" target="_blank" rel="noreferrer noopener">jingyi wei</a>, <a href="https://www.linkedin.com/in/peter-lotfy-ba045684/" target="_blank" rel="noreferrer noopener">peter lotfy</a>, <b>kian faizi</b>, <a href="https://twitter.com/EleanorWang" target="_blank" rel="noreferrer noopener">eleanor wang</a>, <a href="https://www.linkedin.com/in/slabodkin/" target="_blank" rel="noreferrer noopener">hannah slabodkin</a>, emily kinnaman, <a href="https://www.linkedin.com/in/sita-c-990a40171/" target="_blank" rel="noreferrer noopener">sita chandrasekaran</a>, hugo kitano, <a href="https://scholar.google.com/citations?user=hUi_OqkAAAAJ" target="_blank" rel="noreferrer noopener">matthew g. durrant</a>, <a href="https://scholar.google.com/citations?user=0vx-lmkAAAAJ&hl=en&oi=ao" target="_blank" rel="noreferrer noopener">connor v. duffy</a>, <a href="https://bioeng.berkeley.edu/faculty/patrick-hsu" target="_blank" rel="noreferrer noopener">patrick d. hsu</a>, <a href="https://biochemistry.stanford.edu/silvana-konermann" target="_blank" rel="noreferrer noopener">silvana konermann</a>
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
                  i helped conduct a 127,000-guide CRISPR-Cas13d screen to identify guide RNA design rules and optimize transcriptome editing efficiency.
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
                <a href="https://www.linkedin.com/in/illiaziamtsov/" target="_blank" rel="noreferrer noopener">illia ziamtsov</a>, <b>kian faizi</b>, <a href="https://www.cshl.edu/research/faculty-staff/saket-navlakha/" target="_blank" rel="noreferrer noopener">saket navlakha</a>
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
                  i assisted in the development of a software package for plant phenotyping, with a focus on accurate skeleton graph extraction from noisy 3D point clouds.
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
                <b>kian faizi</b>, <a href="https://scholar.google.com/citations?user=heUMphcAAAAJ&hl=en&oi=ao" target="_blank" rel="noreferrer noopener">matthieu platre</a>, <a href="https://www.arjun-chandrasekhar-teaching.com" target="_blank" rel="noreferrer noopener">arjun chandrasekhar</a>, <a href="https://www.cshl.edu/research/faculty-staff/saket-navlakha/" target="_blank" rel="noreferrer noopener">saket navlakha</a>, <a href="https://www.salk.edu/scientist/wolfgang-busch/" target="_blank" rel="noreferrer noopener">wolfgang busch</a>
                <br>
                <!-- <input type="checkbox" id="trigger3">
                <label for="trigger3"><a id="fakelink">abstract</a></label>
                <span id="box">
                  <b>rootmarker</b> is a Python GUI for manually segmenting 2D scans of plant roots. Users point and click to place nodes, creating a skeletonized graph that describes the root system architecture. Includes support for annotating time-series GIFs.
                </span> / -->
                [<a href="https://github.com/kfaizi/ariadne" title="ariadne on GitHub" target="_blank" rel="noreferrer noopener">code</a>]
                <p></p>
                <p>
                  i developed `ariadne`, a time-series image segmentation tool for root phenotyping, and used it to measure pareto-optimal trade-offs in root growth.
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
                  i built a basic workflow for predicting functional homologs of genes driving plant root growth, via co-expression network analysis of single-cell RNA-seq data.
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
                  i programmed a toy model of the <i>lac</i> operon as an asynchronous boolean network, and simulated gene knockout and overexpression experiments. class project for <a href="https://ccom.ucsd.edu/~acloninger/111A_F20/teachingMath111A.html" target="_blank" rel="noreferrer noopener">math 111A</a>.
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
                <b>kian faizi</b>, <a href="https://biochemistry.stanford.edu/silvana-konermann" target="_blank" rel="noreferrer noopener">silvana konermann</a>, <a href="https://bioeng.berkeley.edu/faculty/patrick-hsu" target="_blank" rel="noreferrer noopener">patrick hsu</a>
                <br>
                [<a href="/assets/kian-faizi-srs-2019.pdf" title="srs-2019" target="_blank" rel="noreferrer noopener">poster</a>] /
                [<a href="https://github.com/kfaizi/CRISPR-search" title="CRISPR-search on GitHub" target="_blank" rel="noreferrer noopener">code</a>]
                <p></p>
                <p>
                  i wrote a python pipeline to mine new orthologs of CRISPR-Cas13d from publicly available metagenomic sequence data at terabyte scale.
                </p>
              </td>
            </tr>
          </tbody>
        </table>

        <!-- classes -->
        <h2>teaching</h2>
        <table class="index">
          <tbody>
            <tr>
              <td class="project-media">
                <img class="project-img" src="/assets/images/sisyphus-titian.jpg" title="one must imagine teaching assistants happy" alt="love">
              </td>
              <td class="project-info">
                <p>
                  helping people learn is one of my favorite things in the world. in the future, i'd like to compile a list of tools and resources that have helped me get better at doing it. for now, here's a list of classes i've helped teach, as well as any formal feedback I've received:
                </p>

                <p></p>

                <span class="project-title">bi 1: the great ideas of biology</span>, caltech, spring 2023
                <br>
                head graduate teaching assistant. [<a href="/assets/images/bi1-2023.png">student evaluations</a>] / [<a href="https://bi1.caltech.edu/2023/" target="_blank" rel="noreferrer noopener">course website i made</a>]
                
                <p></p>

                <span class="project-title">bi 1: principles of biology</span>, caltech, spring 2022
                <br>
                graduate teaching assistant. [<a href="/assets/images/bi1-2022.png">student evaluations</a>]
                
                <p></p>

                <span class="project-title"><a href="https://www.ucsd.edu/catalog/courses/BIOL.html#bicd102" target="_blank" rel="noreferrer noopener">bicd 102: genetic inquiry</a></span>, ucsd, fall 2020
                <br>
                undergraduate instructional assistant. [<a href="/assets/Faizi_Kian_Student_IA_Evaluation_BICD_102_FA20.pdf" target="_blank" rel="noreferrer noopener">student evaluations</a>] / [<a href="/assets/Faizi_Kian_Instructor_IA_Evaluation_BICD_102_FA20.pdf" target="_blank" rel="noreferrer noopener">professor's evaluation</a>]
              </td>
            </tr>

          </tbody>
        </table>

      </td>
    </tr>
  </tbody>
</table>


