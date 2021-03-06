---
layout: default
title: Building HTML5 Apps
---

<header>
  <nav>
    <ul>
      <li><a href="#syllabus">Syllabus</a></li>
      <li><a href="#slides">Slides</a></li>
      <li><a href="#examples">Examples</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#resources">Resources</a></li>
    </ul>
  </nav>
  <h1>
    Building
    <img class="html5-logo" src="/img/html5_logo.jpg" alt="HTML5" />
    Web Apps
  </h1>
</header>

<section id="syllabus">
  <div class="container">  
    <h1>Syllabus</h1>
    <h2>Course Info</h2> 
    <ul class="info">
      <li>98-177 Spring 2012</li>
      <li>Tues. 6:30pm - 7:20pm</li>
      <li>Wean Hall 7500</li>
    </ul>
    <h2>Instructors</h2>
    <ul class="info">
      <li><a href="mailto:msamuels@cmu.edu">Molly Samuels</a> &amp; <a href="mailto:brian.a.yee+bh5a@gmail.com">Brian Yee</a></li>
      <li>Office hours by appointment</li>
    </ul>
    <h2>Grading</h2>
    <p>This course is pass/fail (woohoo!)</p>
    <ul class="grading">
      <li><label>Project 1</label> 30%</li>
      <li><label>Final Project</label> 40%</li>
      <li><label>Attendance*</label> 30%</li>
    </ul>
    <p class="footnote">*Missing more than 3 class sessions will result in a big ol&#146; fail whale.</p>
    <h2>Readings</h2>
    <p>On the schedule below, you&#146;ll find a reading that goes along with each class meeting. Readings are not required, but definitely encouraged!</p>
    <h2>Schedule</h2>
    <ul class="card-list">
      <li>
        <label>Jan 17</label>
        <span class="topic">Introduction</span>
        <span class="work"></span>
      </li>
      <li>
        <label>Jan 24</label>
        <span class="topic">Semantic HTML</span>
        <span class="work"><a class="external" href="http://diveintohtml5.info/semantics.html" target="_blank">Ch. 3 (Dive into HTML5)</a></span>
      </li>
      <li>
        <label>Jan 31</label>
        <span class="topic">CSS3</span>
        <span class="work">Ch. 1 (CSS3 for Web Designers)</span>
      </li>
      <li>
        <label>Feb 7</label>
        <span class="topic">HTML5, Flash, and the Battle for Faster Cat Videos</span>
        <span class="work">Google Tech Talk!</span>
      </li>
      <li>
        <label>Feb 14</label>
        <span class="topic">More CSS3</span>
        <span class="work">Ch. 2 (CSS3 for Web Designers)</span>
      </li>
      <li>
        <label>Feb 21</label>
        <span class="topic">Responsive Web Design</span>
        <span class="work"><a class="external" href="http://www.alistapart.com/articles/responsive-web-design/" target="_blank">&#147;Responsive Web Design&#148; by Ethan Marcotte</a>, 
        <strong>Project 1 due</strong>
        </span>
      </li>
      <li>
        <label>Feb 28</label>
        <span class="topic">Audio &amp; Video APIs</span>
        <span class="work"><a class="external" href="http://diveintohtml5.info/video.html" target="_blank">Ch. 5 (Dive in HTML5)</a></span>
      </li>
      <li>
        <label>Mar 6</label>
        <span class="topic">Geolocation API</span>
        <span class="work"><a class="external" href="http://diveintohtml5.info/geolocation.html" target="_blank">Ch. 6 (Dive in HTML5)</a></span>
      </li>
      <li class="unreleased">
        <label>Mar 12</label>
        <span class="topic">NO CLASS</span>
        <span class="work">(Spring Break)</span>
      </li>
      <li>
        <label>Mar 20</label>
        <span class="topic">HTML5 Touch Interfaces</span>
        <span class="work"><a class="external" href="http://www.youtube.com/watch?v=lcD9CF0bxyk" target="_blank">Stephen Woods: Creating Responsive HTML5 Touch Interfaces</a></span>
      </li>
      <li>
        <label>Mar 27</label>
        <span class="topic">History API &amp; AJAX</span>
        <span class="work"><a class="external" href="http://diveintohtml5.info/history.html" target="_blank">Ch. 11 (Dive in HTML5)</a></span>
      </li>
      <li>
        <label>Apr 3</label>
        <span class="topic">Local storage &amp; Offline Apps</span>
        <span class="work"><a class="external" href="http://diveintohtml5.info/storage.html" target="_blank">Ch. 7</a> &amp; <a class="external" href="http://diveintohtml5.info/offline.html" target="_blank">Ch. 8</a> (Dive in HTML5)</span>
      </li>
      <li>
        <label>Apr 10</label>
        <span class="topic">Trendy Tuesday: Parallax &#146;n stuff</span>
        <span class="work"></span>
      </li>
      <li>
        <label>Apr 17</label>
        <span class="topic">Intro to Canvas</span>
        <span class="work"><a class="external" href="http://diveintohtml5.info/canvas.html" target="_blank">Ch. 4 (Dive in HTML5)</a></span>
      </li>
      <li>
        <label>Apr 24</label>
        <span class="topic">In-class work session</span>
        <span class="work"></span>
      </li>
      <li>
        <label>May 1</label>
        <span class="topic">Final Presentations</span>
        <span class="work"><strong>Final Project Due</strong></span>
      </li>
    </ul>
  </div>
</section>

<section id="slides">
  <div class="container">
    <h1>Slides</h1>
    <ul class="card-list">
    {% for post in site.categories.slides reversed %}
      {% if post.hide %}
      <li class="unreleased">
        <label>{{ post.date | date: "%b %d" }}</label>
        <span class="topic">{{ post.title }}</span>
      </li>
      {% else %}
      <li>
        <label>{{ post.date | date: "%b %d" }}</label>
        <a href="{{ post.url }}" class="topic">{{ post.title }}</a>
      </li>
      {% endif %}
    {% endfor %}
    </ul>
  </div>
</section>

<section id="examples">
  <div class="container">
    <h1>Examples</h1>
    <p>Any demos from class will be posted here.</p>
    <ol class="card-list">
      <li><a href="/examples/buttons">Buttons (week 1)</a></li>
      <li><a href="/files/gallery.zip">Gallery Site HTML (week 2)</a></li>
      <li><a href="/files/gallery-week3.zip">Gallery Site w/ CSS (week 3)</a></li>
      <li><a href="/files/candy.html">Candy buttons CSS3 demo (week 5)</a></li>
      <li><a href="/files/geo-demo">Geolocation demo (week 6)</a></li>
      <li><a href="http://diveintohtml5.info/examples/history/adagio.html">History api demo (week 8)</a></li>
      <li><a href="/files/parallax">Parallax demo (week 11)</a></li>
      <li><a href="https://developer.mozilla.org/en/Canvas_tutorial" target="_blank">MDN Canvas tutorial (week 12)</a></li>
    </ol>
  </div>
</section>

<section id="projects">
  <div class="container">
    <h1>Projects</h1>
    <p>Stayed tuned for more details and project requirements.</p>
    <ul class="card-list">
      <li>
        <label>due Feb 21</label>
        <span class="topic">Project 1: Gallery Site</span>
      </li>
      <li>
        <label>due May 1</label>
        <span class="topic">Final Project: Student Choice</span>
      </li>
    </ul>
  </div>
</section>

<section id="resources">
  <div class="container">
    <h1>Resources</h1>
    <p>Found a link you want to share with the class? <a href="mailto:msamuels@cmu.edu">Let us know!</a></p>
    <ul class="card-list">
      <li>
        <a href="http://diveintohtml5.info" target="_blank">Dive into HTML5</a> &ndash; This will serve as our course &#147;textbook&#148;
      </li>
      <li>
        <a href="http://html5forwebdesigners.com" target="_blank">HTML5 For Web Designers</a> &ndash; A brief book by Jeremy Keith
      </li>
      <li>
        <a href="http://www.html5rocks.com/en/" target="_blank">HTML5 Rocks</a> &ndash; A resource for HTML5 developers (from Google)
      </li>
      <li>
        <a href="http://css3.info" target="_blank">CSS3.info</a> &ndash; Everything you need to know about CSS3
      </li>
      <li>
        <a href="http://caniuse.com/" target="_blank">When Can I Use...</a> &ndash; Compatibility tables for support of HTML5, CSS3, SVG, and more in desktop and mobile browsers
      </li>
      <li>
        <a href="http://html5readiness.com" target="_blank">HTML5 &amp; CSS3 Readiness</a> &ndash; Sleak graph version of Can I Use... info
      </li>
      <li>
        <a href="https://developer.mozilla.org/en-US/demos/tag/tech:html5/" target="_blank">Mozilla Demo Studio</a> &ndash; Cool HTML5/CSS3 implementations
      </li>
      <li>
        <a href="http://html5please.us/" target="_blank">HTML5 Please</a> &ndash; Look up HTML5, CSS3, etc features, know if they are ready for use, and if so find out how you should use them (<em>Thanks, Donald Huh!</em>)
      </li>
      <li>
        <a href="http://learn.shayhowe.com/html-css/terminology-syntax-intro/" target="_blank">A Beginners Guide to HTML &amp; CSS</a> &ndash; Beautiful resource for those new to web development!
      </li>
      <li><a href="http://pea.rs/" target="_blank">Pea.rs</a> &ndash; Common patterns (lists, buttons, tabs) and the code that makes them.</li>  
      <li><a href="http://www.benjaminkeen.com/misc/bricss/" target="_blank">Responsive Design Test Bookmarklet</a></li>
      <li><a href="http://www.smashingmagazine.com/2011/07/22/responsive-web-design-techniques-tools-and-design-strategies/" target="_blank">Responsive Web Design Techniques, Tools and Design Strategies</a></li>
    </ul>
  </div>
</section>