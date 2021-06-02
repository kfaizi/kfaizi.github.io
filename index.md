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
<table>
  <tbody>
    <tr style="padding:0px">
      <td style="padding:0px">

        <!-- Introduction -->
        <table id="intro-table">
          <tbody>
            <tr style="padding:0px">
              <td style="width:63%;vertical-align:middle;">
                <p style="text-align:center">
                  <h1 style="text-align: center;">Kian Faizi</h1>
                </p>
              </td>
              <td>
              </td>
            </tr>
            <tr style="padding:0px">
              <td style="padding:2.5%;width:63%;vertical-align:top">
                <p>
                  Hi there! :wave: I'm a senior at <a href="https://www.ucsd.edu" target="_blank" rel="noreferrer noopener">UC San Diego</a> studying molecular biology and math, and an incoming PhD student at <a href="https://www.caltech.edu" target="_blank" rel="noreferrer noopener">Caltech</a> in the systems biology track.
                </p>
                <p>
                  I want to understand how cells make decisions, and reprogram them to do useful things for people and the planet.
                </p>
                <p>
                  Feel free to reach me by
                  <input type="checkbox" id="trigger-e">
                  <label for="trigger-e"><a id="fakelink">email</a></label>.
                  <span id="box"><span class="inline-code">xsnvmv@hpfq.rqh</span> (ROT13)</span>
                  I'm also on <a href="https://www.twitter.com/kianfaizi/" target="_blank" rel="noreferrer noopener">Twitter</a> and <a href="https://www.github.com/kfaizi/" target="_blank" rel="noreferrer noopener">GitHub</a>.
                </p>
              </td>
              <!-- <td style="max-width:37%;vertical-align:text-top;">
                <a href="/assets/images/figtree-headshot.jpg" id="headshot"><img alt="headshot" src="/assets/images/figtree-headshot.jpg"></a>
              </td> -->
            </tr>
          </tbody>
        </table>

        <!-- Blog -->
        <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
          <tbody>
            <tr>
              <td style="padding:20px;width:100%;vertical-align:top">
                <heading>Blog</heading>
                <p>
                  <a href="/blog.html">Sometimes I write</a> about science, programming, and anything else I'm currently curious about. Check out my most recent posts below:
                </p>
                <ul>
                  {% for post in site.posts limit:5 %}
                    <li>
                      <a href="{{ post.url }}">{{ post.title }}</a> <span id="post-date">({{ post.date | date: "%-m/%-d/%y" }})</span>
                    </li>
                  {% endfor %}
                </ul>
              </td>
            </tr>
          </tbody>
        </table>

        <!-- Research interests -->
        <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
          <tbody>
            <tr>
              <td style="padding:5px 20px;width:100%;vertical-align:top">
                <heading>Research</heading>
                <p>
                  I'm interested in <highlight>synthetic biology</highlight>, <highlight>cellular information processing</highlight>, and <highlight>biomolecular computation</highlight>, especially as applied to solving human and environmental problems. I'm currently a tech in <a href="https://www.busch.salk.edu/" target="_blank" rel="noreferrer noopener">Dr. Wolfgang Busch’s</a> plant genetics group at the <a href="https://www.salk.edu/" target="_blank" rel="noreferrer noopener">Salk Institute</a>, where I study root-environment interactions in <i>Arabidopsis thaliana</i> using quantitative and computational methods. A major goal of this research is to aid crop engineering efforts that will <a href="https://www.salk.edu/science/power-of-plants/" target="_blank" rel="noreferrer noopener">fight climate change</a>. Before that, I worked in <a href="http://www.patrickhsulab.org/" target="_blank" rel="noreferrer noopener">Dr. Patrick Hsu's</a> lab, where I helped develop CRISPR-Cas13d for programmable RNA editing.

                  <!-- Representative projects are <span class="highlight">highlighted</span>. -->

                </p>
              </td>
            </tr>
          </tbody>
        </table>

        <!-- Publications and projects -->
        <table>
          <tbody>

            <!-- pub -->
            <tr>
              <td class="project-media">
                <img class="project-img" src="/assets/images/wiring.png" alt="wiring" title="you may think this is too simplified, and you'd be right">
              </td>
              <td class="project-info">
                <span class="project-title">A Boolean Network Model of the Bacterial <i>lac</i> Operon</span>
                <br>
                <highlight>Kian Faizi</highlight>
                <br>
                <a href="https://github.com/kfaizi/boolean-lac" title="boolean-lac on GitHub" target="_blank" rel="noreferrer noopener">code</a>
                <p></p>
                <p>
                  I programmed a toy model of the <i>lac</i> operon as an asynchronous Boolean network, and simulated gene knockout and overexpression experiments. Class project for MATH 111A.
                </p>
              </td>
            </tr>

            <!-- pub -->
            <tr>
              <td class="project-media">
                <img class="project-img" src="/assets/images/p3d.png" alt="p3d" title="meshes are boring (this message brought to you by the point cloud gang)">
              </td>
              <td class="project-info">
                <span class="project-title">Curve Skeleton Extraction from 3D Point Clouds for High-Throughput Plant Phenotyping</span>
                <br>
                <a href="https://www.linkedin.com/in/illiaziamtsov/" target="_blank" rel="noreferrer noopener">Illia Ziamtsov</a>, <highlight>Kian Faizi</highlight>, <a href="https://www.cshl.edu/research/faculty-staff/saket-navlakha/" target="_blank" rel="noreferrer noopener">Saket Navlakha</a>
                <br>
                <i>manuscript in preparation</i>
                <br>
             <!--    <input type="checkbox" id="trigger5">
                <label for="trigger5"><a id="fakelink">abstract</a></label>
                <span id="box">
                  Abstract.
                </span> -->
                <p></p>
                <p>
                  I assisted in the development of a software package for plant phenotyping from noisy 3D point clouds produced from LiDAR scans.
                </p>
              </td>
            </tr>

            <!-- pub -->
            <tr>
              <td class="project-media">
                <img class="project-img" src="/assets/images/coexpression.png" alt="coexpression" title="but is your network scale free though?">
              </td>
              <td class="project-info">
                <span class="project-title">Predicting Functional Homologs from Single-Cell Coexpression Networks</span>
                <br>
                <highlight>Kian Faizi</highlight>, <a href="https://www.salk.edu/scientist/wolfgang-busch/" target="_blank" rel="noreferrer noopener">Wolfgang Busch</a>
                <br>
    <!--             <input type="checkbox" id="trigger4">
                <label for="trigger4"><a id="fakelink">abstract</a></label>
                <span id="box">
                  Abstract.
                </span> / -->
                <a href="https://github.com/kfaizi/coexpression-analysis" title="coexpression-analysis on GitHub" target="_blank" rel="noreferrer noopener">code</a>
                <p></p>
                <p>
                  I built a basic workflow for predicting functional homologs of genes driving plant root growth, via coexpression analysis of single-cell RNA-seq data.
                </p>
              </td>
            </tr>

            <!-- pub -->
            <tr>
              <td class="project-media">
                <img class="project-img" src="/assets/images/rootmarker.png" alt="rootmarker" title="skeletonization go brrrr">
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
                <a href="https://github.com/kfaizi/test-roots" title="test-roots on GitHub" target="_blank" rel="noreferrer noopener">code</a>
                <p></p>
                <p>
                  I developed an image segmentation tool for root phenotyping, and used it to measure cost-performance trade-offs in root growth.
                </p>
              </td>
            </tr>

            <!-- pub -->
            <tr>
              <td class="project-media">
                <img class="project-img" src="/assets/images/screen.png" alt="screen" title="yeah, those are supposed to be cells">
              </td>
              <td class="project-info">
                <span class="project-title">A Pooled CRISPR-Cas13d Screen Reveals Guide RNA Design Principles</span>
                <br>
                <a href="https://biochemistry.stanford.edu/silvana-konermann" target="_blank" rel="noreferrer noopener">Silvana Konermann</a>, <highlight>Kian Faizi</highlight>, <a href="https://www.linkedin.com/in/peter-lotfy-ba045684/" target="_blank" rel="noreferrer noopener">Peter Lotfy</a>, <a href="https://bioeng.berkeley.edu/faculty/patrick-hsu" target="_blank" rel="noreferrer noopener">Patrick Hsu</a>
                <br>
                <i>manuscript in preparation</i>
                <br>
  <!--               <input type="checkbox" id="trigger2">
                <label for="trigger2"><a id="fakelink">abstract</a></label>
                <span id="box">
                  Abstract.
                </span> / -->
                <a href="https://www.nature.com/articles/nprot.2017.016" title="Joung 2017" target="_blank" rel="noreferrer noopener">image credit</a>
                <p></p>
                <p>
                  I helped conduct a 150,000-guide CRISPR-Cas13d screen to identify guide RNA efficiency rules and optimize transcriptome editing efficiency.
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
             <!--    <input type="checkbox" id="trigger1">
                <label for="trigger1"><a id="fakelink">abstract</a></label>
                <span id="box">
                  <b>CRISPRminer</b> is a Python pipeline for discovering novel Cas protein variants from metagenomic data. Putative orthologs are identified with <span class="inline-code">TBLASTN</span>, screened for arrays with <span class="inline-code">CRISPRFinder</span>, and filtered by size, distance, and sequence identity.
                </span> / -->
                <a href="/assets/kian-faizi-srs-2019.pdf" title="srs-2019" target="_blank" rel="noreferrer noopener"> poster</a> /
                <a href="https://github.com/kfaizi/CRISPR-search" title="CRISPR-search on GitHub" target="_blank" rel="noreferrer noopener">code</a>
                <p></p>
                <p>
                  I wrote a Python pipeline to mine new orthologs of CRISPR-Cas13d from publicly available metagenomic sequence data at terabyte scale.
                </p>
              </td>
            </tr>
          </tbody>
        </table>


        <!-- teaching header -->
        <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
          <tbody>
            <tr>
              <td style="padding:5px 20px;width:100%;vertical-align:top">
                <heading>Teaching</heading>
              </td>
            </tr>
          </tbody>
        </table>

        <!-- classes -->
        <table>
          <tbody>
            <tr>
              <td class="project-media">
                <img class="project-img" src="/assets/images/sisyphus-titian.jpg" title="one must imagine teaching assistants happy" alt="love">
              </td>
              <td class="project-info">
                <span class="project-title"><a href="https://www.ucsd.edu/catalog/courses/BIOL.html#bicd102" target="_blank" rel="noreferrer noopener">BICD 102: Genetic Inquiry</a></span>, UCSD, Fall 2020
                <br>
                See evaluations from: <a href="/assets/Faizi_Kian_Student_IA_Evaluation_BICD_102_FA20.pdf" target="_blank" rel="noreferrer noopener">my students</a> / <a href="/assets/Faizi_Kian_Instructor_IA_Evaluation_BICD_102_FA20.pdf" target="_blank" rel="noreferrer noopener">the professor</a>
              </td>
            </tr>

          </tbody>
        </table>

        <!-- etc -->
        <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
          <tbody>
            <tr>
              <td style="padding:5px 20px;width:100%;vertical-align:top">
                <heading>etc</heading>
                <p>
                  Some stuff I like to do <a href="/fun.html">for fun</a>.
                </p>
              </td>
            </tr>
          </tbody>
        </table>

        <!-- Acknowledgements -->
        <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
          <tbody>
            <tr>
              <td style="padding:5px 20px;width:100%;vertical-align:top">
                <heading>Acknowledgements</heading>
                <p>
                  My homepage layout is inspired by <a href="https://jonbarron.info" target="_blank" rel="noreferrer noopener">this ubiquitous website</a>.
                </p>
              </td>
            </tr>
          </tbody>
        </table>



      </td>
    </tr>
  </tbody>
</table>


