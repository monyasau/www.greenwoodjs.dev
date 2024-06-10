---
title: Greenwood
imports:
  - ../components/hero-banner/hero-banner.js data-gwd-opt="static"
  - ../components/footer/footer.js data-gwd-opt="static"
  - ../components/latest-post/latest-post.js data-gwd-opt="static"
  - ../components/walkthrough/walkthrough.js
  - /node_modules/prism-themes/themes/prism-nord.css
  - ../styles/theme.css
  - ../styles/main.css
---

<!-- TODO should probably come from shared layout? -->
<style>
  section.top {
    display: block;
    margin: 0 auto;
    width: 60%;
  }

  .walkthrough-card {
    display: none;
  }
</style>

<section class="top">

<app-latest-post
    link="/blog/release/v0.30.0/"
    title="We just launched v0.30.0">
</app-latest-post>

<app-hero-banner></app-hero-banner>

<app-walkthrough></app-walkthrough>

  <div class="walkthrough-card card1">
    <span>HTML First</span>
    <p>Greenwood is HTML first by design.  Start from just an <i>index.html</i> file or leverage hybrid, file-system based routing to easily achieve static and dynamic pages side-by-side.  Markdown is also supported.</p>

```html
<h1>Hello World!</h1>
```

  </div>

  <div class="walkthrough-card card2">
    <span>CSS Second</span>
    <p>Yay CSS!</p>

```css
h3 {
  color: red;
}
```

  </div>

  <div class="walkthrough-card card3">
    <span>JS Second</span>
    <p>Yay JavaScript</p>

```js
console.log("hello world!");
```

  </div>

  <div class="walkthrough-card card4">
    <span>And lastly...</span>
    <p>Yay Greenwood!</p>

```js
new Response("<h3>Hello World</h3>", { headers: { "Content-Type": "text/html" } });
```

  </div>

<app-footer></app-footer>

</section>
