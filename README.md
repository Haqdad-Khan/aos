<!-- This guide is made by Haqdad Khan. (github.com/haqdadkhan) -->

# Animation on Scroll - Notes

<p>This is my Personal Guide to learn <code>AOS - Library</code> for creative and cutting-edge Web Designs.</p>

<!-- Installation -->
## Installation:

<!-- For HTML -->
### CDN Sources
<p>Add these links to your <code>index.html</code>.</p>
<p>CSS</p>
    <pre>&lt;link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet"&gt;</pre>
<p>JS</p>
    <pre>&lt;script src="https://unpkg.com/aos@2.3.1/dist/aos.js"&gt; &lt;/script&gt;</pre>

<!-- For React -->
### Install using Yarn, Npm, Bower
<pre>yarn add aos</pre>
<pre>npm install aos --save</pre>
<pre>bower install aos --save</pre>

<!-- AOS in HTML -->
### AOS in HTML

<!-- script.js -->
<p>Create a <code>script.js</code> and paste the following <code>code</code> to use <code>AOS</code>.</p>
<pre>
&lt;script&gt;
    AOS.init();
&lt;/script&gt;
</pre>

<!-- index.html -->
<p>You simply need to put a <code>data-aos="desired_property"</code> as a attribute in your <b>HTML Element/Tag</b> to use <code>AOS</code>.</p>

<pre>
&lt;!DOCTYPE html&gt;
&lt;html lang="en"&gt;
&lt;head&gt;
    &lt;meta charset="UTF-8"&gt;
    &lt;meta name="viewport" content="width=device-width, initial-scale=1.0"&gt;
    &lt;title&gt;Learn Animation on Scroll&lt;/title&gt;
    &lt;!-- stylesheet --&gt;
    &lt;link rel="stylesheet" href="style.css"&gt;
&lt;/head&gt;
&lt;body&gt;
    &lt;h1&gt;Welcome to AOS Tutorial.&lt;/h1&gt;
    &lt;p data-aos="fade-up"&gt;This is a complete guide to install and use <b>AOS</b>.&lt;/p&gt;
    &lt;!-- javascript --&gt;
    &lt;script src="script.js"&gt;&lt;/script&gt;
&lt;/body&gt;
&lt;/html&gt;
</pre>

<!-- AOS in React -->
### AOS in React

<!-- App.jsx -->
<p>You will initialize <code>AOS</code> in your <b>React</b> project in <code>index.js/App.js</code>. In case of <b>Vite React</b> file names could vary as <code>main.jsx/App.jsx</code>.</p>

<pre>
import AOS from 'aos';
import 'aos/dist/aos.css';
import Component from './components/Component';
import { useEffect } from 'react';

function App() {
  // initializing AOS
  useEffect(() =&gt; {
    AOS.init();
  }, [])

  return (
    &lt;&gt;
      &lt;Component /&gt;
    &lt;/&gt;
  )
}

export default App;
</pre>

<!-- Component.jsx -->
<p>Create a <code>Component.js</code> and paste the following <code>code</code> to use <code>AOS</code> with a component.</p>

<pre>
import React from 'react';

function Component() {
    return (
        &lt;div data-aos="fade-left"&gt;Component&lt;/div&gt;
    );
}

export default Component;
</pre>

## Table of Contents:

<ol>
    <li><a href="#fade-anim">Fade Animation</a></li>
    <li><a href="#flip-anim">Flip Animation</a></li>
    <li><a href="#slide-anim">Slide Animation</a></li>
    <li><a href="#zoom-anim">Zoom Animation</a></li>
</ol>

---

<section id="fade-anim">
<h2> Fade Animation</h2>

- Fade up: <code>data-aos="fade-up"</code>
- Fade down: <code>data-aos="fade-down"</code>
- Fade right: <code>data-aos="fade-right"</code>
- Fade left: <code>data-aos="fade-left"</code>
- Fade p right: <code>data-aos="fade-up-right"</code>
- Fade up left: <code>data-aos="fade-up-left"</code>
- Fade down right: <code>data-aos="fade-down-right"</code>
- Fade down left: <code>data-aos="fade-down-left"</code>
</section>

---

<section id="flip-anim">
<h2> Flip Animation</h2>

- Flip up: <code>data-aos="flip-up"</code>
- Flip down: <code>data-aos="flip-down"</code>
- Flip right: <code>data-aos="flip-right"</code>
- Flip left: <code>data-aos="flip-left"</code>
</section>

---

<section id="slide-anim">
<h2> Slide Animation</h2>

- Slide up: <code>data-aos="slide-up"</code>
- Slide down: <code>data-aos="slide-down"</code>
- Slide right: <code>data-aos="slide-right"</code>
- Slide left: <code>data-aos="slide-left"</code>
</section>

---

<section id="zoom-anim">
<h2> Zoom Animation</h2>

- Zoom in: <code>data-aos="zoom-in"</code>
- Zoom out: <code>data-aos="zoom-out"</code>
- Zoom in up: <code>data-aos="zoom-in-up"</code>
- Zoom in down: <code>data-aos="zoom-in-down"</code>
- Zoom in left: <code>data-aos="zoom-in-left"</code>
- Zoom in right: <code>data-aos="zoom-in-right"</code>
- Zoom out up: <code>data-aos="zoom-out-up"</code>
- Zoom out down: <code>data-aos="zoom-out-down"</code>
- Zoom out left: <code>data-aos="zoom-out-left"</code>
- Zoom out right <code>data-aos="zoom-out-right"</code>
</section>

---