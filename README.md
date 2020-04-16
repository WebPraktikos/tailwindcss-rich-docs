Tailwind CSS Rich Docs
---------

**Important:** Still at an early stage of development and not ready for use.

Tailwind CSS plugin that creates styled documentation page from row HTML code.

[Demo](https://tailwindcss-rich-docs.netlify.com/)

**How to use it?**  
Add the `rich-docs` class to the element which wraps raw HTML code (without styles).

**How to use the same font as on the demo site?**  
Add the following code to the `<head>` HTML element:

```html
<link href="https://fonts.googleapis.com/css?family=Fira+Sans:200,200i,300,300i,400,400i,500,500i,600,600i,700,700i,800,800i&display=swap" rel="stylesheet">
```

Setup
---------

Install the `tailwindcss-rich-docs` npm package:
```
npm install tailwindcss-rich-docs
```

Include it in your `tailwind.config.js`:
```
module.exports = {
  theme: {},
  variants: {},
  plugins: [
    require("tailwindcss-rich-docs")
  ]
};
```

Add the `rich-docs` class:
```html
<div class="rich-docs">
  <!-- markdown to html output, maybe -->
</div>
```

Embed a Video
---------

To embed a video iframe or any other iframe, wrap the iframe with a div. Then, add the`iframe-parent` class to that div. Next, specify the aspect ratio under the `style` attribute. Finally, remove width, height, and other styles from the iframe.
```html
<div class="iframe-parent" style="--aspect-ratio-horizontal: 16; --aspect-ratio-vertical: 9;">
  <!-- Example iframe -->
  <iframe src="https://www.youtube.com/embed/MURPf_6r8z4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
```
