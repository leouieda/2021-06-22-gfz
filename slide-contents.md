<!--
This file defines the contents of each slide.
The reveal.js configuration can be found in index.html
-->

<!-- .slide: class="slide-title" data-background-color="#000000" data-background-image="assets/background.svg" data-background-repeat="no-repeat" data-background-position="center" -->

<div class="talk-title">

# Open-science for gravimetry:

## Tools, challenges, and opportunities

</div>

<div class="talk-authors">

### Leonardo Uieda <br> Santiago Soler, Agustina Pesce

</div>

GFZ Helmholtz Centre Potsdam <span style="margin: 0 20px">|</span> 22 June 2021

<img src="assets/compgeolab-banner-light.svg" class="title-logo">
<img src="assets/university-of-liverpool-white.png" class="title-logo">
<img src="assets/conicet.png" class="title-logo">
<img src="assets/universidad-nacional-de-san-juan.png" class="title-logo">

<i class="fab fa-twitter fa-fw"></i> [@leouieda](https://twitter.com/leouieda)
<span style="margin: 0 20px">|</span>
<i class="fa fa-camera"></i>
Feel free to screenshot/share/reuse/remix this presentation
<span style="margin: 0 20px">|</span>
[<i class="fab fa-creative-commons"></i><i class="fab fa-creative-commons-by"></i> CC-BY 4.0 License](https://creativecommons.org/licenses/by/4.0/)

---

<!-- .slide: data-background-image="assets/fatiando-a-terra-front-page.svg" data-background-size="contain" data-background-repeat="no-repeat" data-background-color="#000000" -->

<div class="r-stretch bottom-right">

This talk will be mostly about the [Fatiando a Terra](https://www.fatiando.org)
project.
**Fun fact:** the name is Portuguese for **"Slicing the Earth"**

</div>

---

<!-- .slide: class="slide-transition" data-background-color="#060629" -->

<div class="centered">
<div>

# First, a bit of history

<img src="assets/logo-evolution.svg" style="margin-top: 5%;">

</div>
</div>

---

<!-- .slide: data-background-video="assets/brasil-sao-paulo-rio.mp4" data-background-size="contain" data-background-color="#000000" -->

<div class="r-stretch bottom-right">

Our journey starts in Southeastern Brazil, specifically in São Paulo and Rio de
Janeiro

</div>

---

<!-- .slide: data-background-image="assets/fatiando-as-a-gravmag-gui.svg" data-background-size="contain" data-background-opacity="0.2" data-background-repeat="no-repeat" data-background-color="#ffffff" -->

<div class="centered">
<div class="quote">

Started around 2008 as a GUI for **2D gravity modelling** developed with
fellow **undergrads** at USP, Brazil

</div>
</div>

---

<!-- .slide: data-background-image="assets/fatiando-as-a-gravmag-gui.svg" data-background-size="contain" data-background-repeat="no-repeat" data-background-color="#000000" -->

<div class="r-stretch bottom-right bottom-dark">

Actual diagram of the GUI workflow retrieved from our version control system.

</div>

---

<!-- .slide: data-background-image="assets/fatiando-first-commit.svg" data-background-size="contain" data-background-repeat="no-repeat" data-background-color="#ffffff" data-background-opacity="0.2" -->

<div class="centered">
<div class="quote">

Transitioned into a **Python library**
in 2010
when I started my MSc in Rio working on gravity gradient 3D inversion

</div>
</div>

---

<!-- .slide: data-background-image="assets/fatiando-first-commit.svg" data-background-size="contain" data-background-repeat="no-repeat" data-background-color="#000000" -->

<div class="r-stretch bottom-right">

The exact date and time when this happened is still registered in our git repository
(commit: [928515b](https://github.com/fatiando/fatiando/commit/928515b0fcfdccecbc4f661ed2469390ef43ec1d))

</div>

---

<!-- .slide: data-background-image="assets/fatiando-first-commit-vcs.svg" data-background-size="contain" data-background-repeat="no-repeat" data-background-color="#000000" -->

<div class="r-stretch bottom-right">

**Learned a lot** about software development:
version control (went through 3),
<br>
tests, packaging, documentation, and more.

</div>

---

<!-- .slide: data-background-image="assets/fatiando-first-gallery.jpg" data-background-size="contain" data-background-repeat="no-repeat" data-background-color="#000000" -->

<div class="r-stretch bottom-left bottom-dark">

Around 2011 we built the first website and gallery. We ended up building a 2D
GUI and much more,
<br>
from seismic to potential fields and heat flow.

</div>

---

<!-- .slide: data-background-image="assets/fatiando-docs-v0.1.jpg" data-background-size="contain" data-background-repeat="no-repeat" data-background-color="#000000" -->

<div class="r-stretch bottom-left bottom-dark">

First documentation built using [sphinx](https://www.sphinx-doc.org) for
**v0.1** (2013). doi:[10.5281/zenodo.16207](https://doi.org/10.5281/zenodo.16207)

</div>

---

<!-- .slide: data-background-image="assets/fatiando-docs-v0.5.jpg" data-background-size="contain" data-background-repeat="no-repeat" data-background-color="#000000" -->

<div class="r-stretch bottom-left bottom-dark">

Santiago and other contributors joined and we made several releases until **v0.5** (2016). doi:[10.5281/zenodo.157746](https://doi.org/10.5281/zenodo.157746)

</div>

---

<div class="container">
<div class="col-left" style="padding-right: 5%">

<h1 style="color: #0000dd;">
<i class="far fa-thumbs-up" style="margin-right: 20px;"></i>
The good parts
</h1>

<hr>

<ul class="fa-ul">

<li>
<span class="fa-li"> <i class="fa fa-lightbulb fa-fw"></i> </span>
State-of-the-art algorithms
</li>

<li>
<span class="fa-li"> <i class="fa fa-file-alt fa-fw"></i> </span>
Used in several thesis & papers (>70 citations)
</li>

<li>
<span class="fa-li"> <i class="fa fa-users fa-fw"></i> </span>
2-3 active contributors
</li>

<li>
<span class="fa-li"> <i class="fa fa-chalkboard-teacher fa-fw"></i> </span>
Enabled teaching through simulation
</li>

</ul>

</div>
<div class="col-right fragment" style="padding-left: 5%">

<h1 style="color: #dd0000;">
<i class="far fa-thumbs-down" style="margin-right: 20px;"></i>
The bad parts
</h1>

<hr>

<ul class="fa-ul">

<li>
<span class="fa-li"> <i class="fa fa-gamepad fa-fw"></i> </span>
Too many toy problems and experimental code
</li>

<li>
<span class="fa-li"> <i class="fas fa-vial fa-fw"></i> </span>
Not designed for testability
</li>

<li>
<span class="fa-li"> <i class="fa fa-tools fa-fw"></i> </span>
Difficult to maintain
</li>

<li>
<span class="fa-li"> <i class="fa fa-landmark fa-fw"></i> </span>
Unstable foundations for growth
</li>

</ul>
</div>

---

<div class="container small">
<div class="col">

### ✨ New Fatiando ✨

Split into libraries

Better coding practices

Use modern tools

Supplement the ecosystem

</div>
<div class="col fragment">

<a href="http://www.fatiando.org/pooch">
<img class="project-logo center-block" src="assets/pooch-logo.svg">
</a>

Data <b>download & caching</b> (used by other libraries)

<ul class="fa-ul project-icons">
<li><i class="fa-li fab fa-github fa-fw" title="Github repository"></i>
   <a href="https://github.com/fatiando/pooch">fatiando/pooch</a>
</li>
<li><i class="fa-li fas fa-bookmark fa-fw" title="Publication"></i>
   doi: <a href="https://doi.org/10.21105/joss.01943">10.21105/joss.01943</a>
</li>
<li><i class="fa-li fa fa-check fa-fw" style="color: green" title="Project status"></i>
   Stable and ready for use
</li>
</ul>

</div>
<div class="col fragment">

<a href="http://www.fatiando.org/verde">
<img class="project-logo center-block" src="assets/verde-logo.svg">
</a>

ML-based point data processing and <b>gridding</b>

<ul class="fa-ul project-icons">
<li><i class="fa-li fab fa-github fa-fw" title="Github repository"></i>
   <a href="https://github.com/fatiando/verde">fatiando/verde</a>
</li>
<li><i class="fa-li fas fa-bookmark fa-fw" title="Publication"></i>
   doi: <a href="https://doi.org/10.21105/joss.00957">10.21105/joss.00957</a>
</li>
<li><i class="fa-li fa fa-check fa-fw" style="color: green" title="Project status"></i>
   Stable and ready for use
</li>
</ul>

</div>
</div>
<div class="container small" style="margin-top: 4%">
<div class="col fragment">

<a href="http://www.fatiando.org/harmonica">
<img class="project-logo center-block" src="assets/harmonica-logo.svg">
</a>

Processing and modeling <b>gravity & magnetic</b> data

<ul class="fa-ul project-icons">
<li><i class="fa-li fab fa-github fa-fw" title="Github repository"></i>
   <a href="https://github.com/fatiando/harmonica">fatiando/harmonica</a>
</li>
<li><i class="fa-li fa fa-sync-alt fa-fw" style="color: green" title="Project status"></i>
   Ready for use but still changing
</li>
</ul>

</div>
<div class="col fragment">

<a href="http://www.fatiando.org/boule">
<img class="project-logo center-block" src="assets/boule-logo.svg">
</a>

Reference <b>ellipsoids</b> for <b>normal gravity</b>

<ul class="fa-ul project-icons">
<li><i class="fa-li fab fa-github fa-fw" title="Github repository"></i>
   <a href="https://github.com/fatiando/boule">fatiando/boule</a>
</li>
<li><i class="fa-li fa fa-sync-alt fa-fw" style="color: green" title="Project status"></i>
   Ready for use but still changing
</li>
</ul>

</div>
<div class="col fragment">

<a href="http://www.fatiando.org/rockhound">
<img class="project-logo center-block" src="assets/rockhound-logo.svg">
</a>

Repository for our **sample data** (uses Pooch)

<ul class="fa-ul project-icons">
<li><i class="fa-li fab fa-github fa-fw" title="Github repository"></i>
   <a href="https://github.com/fatiando/rockhound">fatiando/rockhound</a>
</li>
<li><i class="fa-li fa fa-flask fa-fw" style="color: orange" title="Project status"></i>
    Early stages of design
</li>
</ul>

</div>
</div>

---

<!-- .slide: class="slide-transition" data-background-color="#000000" data-background-image="assets/demo-time.gif" data-background-repeat="no-repeat" data-background-position="center" data-background-opacity="70%" -->

<div class="centered">
<div>

# Demo time!

</div>
</div>

---

<!-- .slide: class="slide-transition" data-background-color="#060629" -->

<div class="centered">
<div>

<h1>
Ongoing <br> developments
</h1>

</div>
</div>

---

Slides about:

* EQL work (santi and harmonica)
* Filters
* Boule rewrite
* Docs reorganizing
* Increase recruitment and diversity

---

<!-- .slide: class="slide-transition" data-background-color="#060629" -->

<div class="centered">
<div>

<h1>
Come for the <strong>code</strong> <i class="fas fa-code"></i>
<br>
Stay for the <strong>community</strong> <i class="fas fa-users"></i>
</h1>

</div>
</div>

---

# Get started

<ul class="fa-ul">

<li class="fragment">
<span class="fa-li"><i class="fab fa-python"></i></span>
Not experienced with Python?
<ul style="margin: 1em 0 0 1em;">
<li>
  Software Carpentry has <a href="https://swcarpentry.github.io/python-novice-inflammation/">great open-access lessons</a>
</li>
</ul>
</li>

<li class="fragment">
<span class="fa-li"><i class="fab fa-youtube"></i></span>
Watch some tutorials on YouTube:
<ul style="margin: 1em 0 0 1em;">
<li>
  Verde (<a href="https://www.youtube.com/watch?v=-xZdNdvzm3E">Transform 2020 </a>) and
  Harmonica (<a href="https://www.youtube.com/watch?v=0bxZcCAr6bwab_channel=SoftwareUnderground">Transform 2021</a>)
</li>
</ul>
</li>

<li class="fragment">
<span class="fa-li"> <i class="fas fa-book"></i> </span>
Documentation for each library
(links at <a href="https://www.fatiando.org">fatiando.org</a>)
</li>

</ul>

---

# Get involved

There are many ways to participate:

<div class="container">
<div class="col-left">
<ul>
<li class="fragment">Write code</li>
<li class="fragment">Work on documentation or examples</li>
<li class="fragment">Give feedback</li>
</lu>
</div>
<div class="col-right">
<ul>
<li class="fragment">Join the conversation</li>
<li class="fragment">Share your experience</li>
<li class="fragment">Help guide future development</li>
</ul>
</div>
</div>

<div class="fragment">

**Your help is always welcome!**

</div>

---

# Where to find us

<ul class="fa-ul">

<li class="fragment">
<span class="fa-li"><i class="fab fa-slack"></i></span>
<a href="http://contact.fatiando.org/">Slack</a>:
where we chat about meetings, events, questions, experiences
</li>

<li class="fragment">
<span class="fa-li"><i class="fab fa-github"></i></span>
<a href="https://github.com/fatiando/">GitHub</a>:
where we discuss development details and review code
</li>

<li class="fragment">
<span class="fa-li"><i class="fa fa-microphone-alt"></i></span>
<div class="container">
<div class="col-left">
<a href="https://github.com/fatiando/meeting-notes">Video Calls</a>:
<b>Community Calls</b> (monthly) to socialize and plan,
<b>Development Calls</b> (weekly) to discuss the details
</div>
<div class="col-right">
<img src="assets/fatiando-community-call.jpg">
</div>
</div>
</li>

</ul>

---

<div class="centered huge">
<div>

About Fatiando:
[fatiando.org](https://www.fatiando.org)

Our research:
[compgeolab.org](https://www.compgeolab.org)

Slides + demo:
[github.com/leouieda/2021-06-22-gfz](https://github.com/leouieda/2021-06-22-gfz)

</div>
</div>

---

<!-- .slide: class="slide-license" -->

<div class="centered">
<div>

<p class="license-icons">
<i class="fab fa-creative-commons"></i><i class="fab fa-creative-commons-by"></i>
</p>

Unless otherwise noted,
the contents of this presentation are
licensed under the
<br>
[Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

</div>
</div>
