---
layout: folio
name_zh: 杨声远
affiliation: University of Wisconsin–Madison
position: Ph.D. student in Computer Science
portrait: /images/shengyuanyang-portrait.webp
footer_quote: 这里或那里，世界很大，世界很好。
publications:
  - title: "MBUndo: Sound, Automatic, and Efficient Measurement-Based Uncomputation for Quantum Circuits"
    id: mbundo
    authors: "**Shengyuan Yang** and Charles Yuan."
    venue: arXiv · 2026
    links:
      - label: Preprint
        url: https://arxiv.org/abs/2611.02345
    highlight:
      text: >-
        How can we clean up temporary quantum values without paying the cost of reversing the computation that produced them?
        We present MBUndo, the first compiler pass that performs measurement-based uncomputation automatically.
        It finds when each temporary qubit can safely be measured and then replaces its unitary uncomputation gates with cheap in-place phase corrections.
        Across 22 benchmarks, this transformation used 40% fewer *T* gates than the unitary uncomputation circuits did.
      image: /images/mbundo.webp
      image_width: 3196
      image_height: 794
      image_alt: MBUndo measures temporary qubits after their last use and replaces cleanup gates with phase corrections. In this example, uncomputation drops from 21 T gates to 7.
  - title: The Time-Space Complexity of Checking Multiple Assertions in Quantum Programs
    id: assertion-checking
    authors: "**Shengyuan Yang** and Charles Yuan."
    venue: arXiv · 2026
    links:
      - label: Preprint
        url: https://arxiv.org/abs/2607.11665
    highlight:
      text: >-
        How many program executions or extra qubits do we need to learn the outcomes of *n* assertions in a quantum program?
        We show that the answer hinges on what information we want to extract and characterize the complexity of different tasks.
        The complexity is logarithmic for detecting whether any assertion fails or finding the first failure, and linear for reporting all assertion outcomes.
      image: /images/assertion-checking.webp
      image_width: 3528
      image_height: 796
      image_alt: An example program with three assertions and a table comparing the extra qubits needed to detect any failure, find the first failure, or report all failures across different numbers of runs.
  - title: "Cut-Shortcut Whole-Program Pointer Analysis: Re-imagining Context-Sensitivity without Contexts"
    id: cut-shortcut-s
    authors: "**Shengyuan Yang**, Wenjie Ma, Thomas Reps, Tian Tan, Yue Li."
    venue: TOPLAS ’26
    links:
      - label: Paper
        url: https://dl.acm.org/doi/10.1145/3818615
      - label: Artifact
        url: https://github.com/YangShengYuan/cut-shortcut-artifact
    highlight:
      text: >-
        How can we support modern language features such as streams and their interaction with lambda expressions in pointer analysis for Java?
        We extend the Cut-Shortcut approach to provide a full static model of Java stream behavior that tracks how objects flow through different stream pipelines, enabling precise pointer analysis for Java programs with heavy stream use.
      image: /images/cut-shortcut-s.webp
      image_width: 3344
      image_height: 822
      image_alt: Diagrams compare object flow through two Java stream pipelines, and a Stream.map example shows two method references invoked through shared library code.
  - title: Context Sensitivity without Contexts, A Cut-Shortcut Approach to Fast and Precise Pointer Analysis
    id: cut-shortcut
    authors: "Wenjie Ma#, **Shengyuan Yang#**, Tian Tan, Xiaoxing Ma, Chang Xu, Yue Li."
    author_note: "# Equal contribution."
    venue: PLDI ’23
    venue_title: ACM SIGPLAN Conference on Programming Language Design and Implementation
    links:
      - label: Paper
        url: https://dl.acm.org/doi/abs/10.1145/3591242
      - label: Artifact
        url: https://zenodo.org/record/7808384
    highlight:
      text: >-
        Context-insensitive pointer analysis is fast but imprecise, while context-sensitive pointer analysis is precise yet inefficient. Can we have an approach that offers both benefits?
        We provide Cut-Shortcut, a novel pointer analysis algorithm based on manipulating edges in the pointer-flow graph.
        Cut-Shortcut is even faster than context-insensitive analysis on most benchmarks and achieves precision comparable to that of context-sensitive analysis.
      image: /images/cut-shortcut.webp
      image_width: 3718
      image_height: 902
      image_alt: A Java example shows how Cut-Shortcut keeps the results of two calls to the same method distinct. The chart compares analysis times in Doop across ten Java programs.
  - title: "Quantum Assertion Testing Without Mid-Circuit Measurement: Strategies and Lower Bounds"
    authors: "**Shengyuan Yang**, Charles Yuan."
    venue: PLanQC ’26
    venue_url: https://popl26.sigplan.org/details/planqc-2026-papers/4/Quantum-Assertion-Testing-Without-Mid-Circuit-Measurement-Strategies-and-Lower-Bound
    links:
      - label: Paper
        url: https://yangshengyuan.github.io/file/QAT.pdf
  - title: "Imprompt: A Language Framework for Prompt Programming"
    authors: "Chentian Wu, **Shengyuan Yang**, Adithya Murali."
    venue: arXiv · 2026
    links:
      - label: Preprint
        url: https://arxiv.org/abs/2607.22683
---

<section class="folio-section" id="about-me" aria-labelledby="about-heading" markdown="1">
<h2 id="about-heading">About</h2>
<div class="folio-bio" markdown="1">

I am a fourth-year Ph.D. student in Computer Science at the University of Wisconsin–Madison and a member of the [MadPL Group](https://madpl.cs.wisc.edu/).

I am broadly interested in the principles and techniques of programming languages, and in using them to reason about computing systems and improve their security and efficiency.

My research includes programming language principles and tools for quantum computing, under the supervision of [Charles Yuan](https://pages.cs.wisc.edu/~charlesyuan/). My work explores [time-space trade-offs for checking quantum assertions](https://arxiv.org/abs/2607.11665). My recent work also includes [MBUndo, a sound, automatic, and efficient compiler pass for measurement-based uncomputation](https://arxiv.org/abs/2611.02345) that reduces the cost of uncomputation in quantum circuits.

My earlier research focused on pointer analysis algorithms and their foundations. This work includes [Cut-Shortcut](https://dl.acm.org/doi/10.1145/3591242), a fast and precise approach to pointer analysis for object-oriented languages, and [Cut-Shortcut-S](https://yangshengyuan.github.io/file/CSCS.pdf), which models Java Streams and their interaction with lambda expressions for precise static analysis. At Wisconsin, I earned an M.S. and worked with [Thomas Reps](https://pages.cs.wisc.edu/~reps/) on pointer analysis algorithms. Before coming to Wisconsin, I received both a B.E. and an M.E. in Software Engineering from Nanjing University, where I worked with [Yue Li](https://yuelee.bitbucket.io/) and [Tian Tan](https://silverbullettt.bitbucket.io/) as a member of the [PASCAL Research Group](https://pascal-lab.net/).

I am also interested in programming language support for LLM-based AI systems. In [Imprompt](https://arxiv.org/abs/2607.22683), we designed a structured prompt programming language that separates task descriptions from execution details, together with formal compilation strategies.

<!-- For more information, please see my [résumé](https://yangshengyuan.github.io/file/CV-shengyuanyang.pdf). -->

</div>
</section>

<section class="folio-section" id="publications" aria-labelledby="publications-heading">
  <h2 id="publications-heading">Publications</h2>
  <ul class="folio-paper-list" role="list">
    {% for paper in page.publications %}
    <li class="folio-paper"{% if paper.id %} id="{{ paper.id | escape }}"{% endif %}>
      <div class="folio-venue folio-label"{% if paper.venue_title %} title="{{ paper.venue_title | escape }}"{% endif %}>
        {% if paper.venue_url %}<a href="{{ paper.venue_url | escape }}">{{ paper.venue | escape }}</a>{% else %}{{ paper.venue | escape }}{% endif %}
      </div>
      <h3 class="folio-paper-title">{{ paper.title | escape }}</h3>
      <div class="folio-authors">
        {{ paper.authors | markdownify }}
        {% if paper.author_note %}<p>{{ paper.author_note | escape }}</p>{% endif %}
      </div>
      <div class="folio-paper-links">
        {% for link in paper.links %}
        <a href="{{ link.url | escape }}">{{ link.label | escape }}</a>
        {% endfor %}
      </div>
      {% if paper.highlight %}
      <div class="folio-paper-highlight">
        {{ paper.highlight.text | markdownify }}
        {% if paper.highlight.image %}
        <a class="folio-paper-figure" href="{{ paper.highlight.image | relative_url }}" aria-label="View full-size figure for {{ paper.title | escape }}">
          <img src="{{ paper.highlight.image | relative_url }}" width="{{ paper.highlight.image_width }}" height="{{ paper.highlight.image_height }}" alt="{{ paper.highlight.image_alt | escape }}" loading="lazy">
        </a>
        {% endif %}
      </div>
      {% endif %}
    </li>
    {% endfor %}
  </ul>
</section>

<section class="folio-section" id="services" aria-labelledby="services-heading">
  <h2 id="services-heading">Services</h2>
  <dl class="folio-services">
    <div>
      <dt>Artifact Evaluation Committee</dt>
      <dd>SAS'25, PLDI'26.</dd>
    </div>
    <div>
      <dt>Journal Reviewer</dt>
      <dd>TOSEM.</dd>
    </div>
    <div>
      <dt>Teaching Assistant</dt>
      <dd>Static Analysis (2021 Fall), Java programming (2023 Fall), Introduction to the Theory and Design of Programming Langugaes (2024 Spring, 2024 Fall, 2025 Spring, 2025 Fall)</dd>
    </div>
  </dl>
</section>

<section class="folio-section" id="projects" aria-labelledby="projects-heading" markdown="1">
<h2 id="projects-heading">Projects</h2>
<div class="folio-projects" markdown="1">
<div markdown="1">

### Undergraduate Thesis at Nanjing University
- **Hymers**: a hybrid heap abstraction tool to accelerate pointer analysis by dividing abstract heaps into
different categories to apply corresponding abstraction methods.

</div>
<div markdown="1">

### Master Thesis at Wisconsin-Madison
- **A Static Modeling of Java Streams**: a static modeling of Java streams in pointer analysis, modeling all kinds of stream pipeline operations to track stream input-output relations.

</div>
<div markdown="1">

### Competition Projects
- **A Side-Scrolling Tactical RPG**: a game developed by Unity, lead an 8-person team to win 1st place in *Game Development Contest by Thunder Fire Studio, NetEase & Nanjing University*.
- **Campus Vacant Classroom Wayfinding App**: an Android App using WIFI detection to locate the user's position in buildings, and enabling in-building navigation for vacant classrooms, won 1st place in *hackathon by Academic Collaboration Dept., Microsoft Research Asia & Nanjing University*.

</div>
<div markdown="1">

### Selcted Course Projects
- **OCEANIA**: a web system to visualize the call-graph of a given program uploaded by users. Led a 3-person team and impelemented 2 call-graph construction strategies (a fast code traversal solution and a precise pointer analysis solution).
- **Online Cinema System**: a 2KLOC web system that releases, schedules, and sells tickets for cinema.
- **Online Judge System**: as the scrum manager, help a 4-person team to complete an agile software process in developing an online judge system in 2 sprints, using Zenhub, Kanban and burndown charts.
- **Test Impact Selction Tool**: leveraged static analysis framework WALA to design and implement a tool that selects test cases impacted by a given change.

</div>
</div>
</section>

<section class="folio-section" id="hobbies" aria-labelledby="hobbies-heading" markdown="1">
<h2 id="hobbies-heading">Hobbies</h2>
<div class="folio-hobbies" markdown="1">

- Video Games: Soulsborne, crpg, fire emblem, card games.
- Science Fiction & Detective Novels: Ted Chiang, 小林 泰三, 西泽 保彦, 江户川 乱步, 京极 夏彦
- I'm learning electric guitar

</div>
</section>
