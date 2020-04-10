Tailwind CSS Rich Docs
---------

**Important:** Still at an early stage of development and not ready for use.

This is a Tailwind CSS plugin that adds styles to the raw HTML code (without styles or classes) containing documentation type of content.

[Demo](https://tailwindcss-rich-docs.netlify.com/)

**How to use it?**  
Add the `rich-docs` class to the element which wraps raw HTML code.

**How to use the same font as on the demo site?**  
Add the following code to the `<head>` HTML element:

```html
<link href="https://fonts.googleapis.com/css?family=Fira+Sans:200,200i,300,300i,400,400i,500,500i,600,600i,700,700i,800,800i&display=swap" rel="stylesheet">
```

Setup
---------

Install the tailwindcss-rich-docs npm package:
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
