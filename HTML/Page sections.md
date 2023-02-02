It is important to create a correct structure for the page, because search engines and screen readers use it to read the content of the page and understand its structure. 

## Generic page structure

This is a generic structure of a page. It uses *block-level* elements.

<table>
	<tr><td colspan="2"><code>header</code></td></tr>
	<tr><td colspan="2"><code>nav</code></td></tr>
	<tr>
		<td><code>section</code></td>
		<td rowspan="2"><code>aside</code></td>
	</tr>
	<tr><td><code>article</code></td></tr>
	<tr><td colspan="2"><code>footer</code></td></tr>
</table>

### Header

```html
<header>
  <h1>this is my header</h1>
</header>
```

### Navigation bar

```html
<nav>
  <a href="#">link 1</a>
  <a href="#">link 2</a>
  <a href="#">link 3</a>
</nav>
```

### Main content

```html
<main>
  <article>
    <h2>some heading</h2>
    <p>some text</p>
  </article>
</main>
```

### Article and section

`<section>` is similar to `<article>`, but it is used for grouping together a single part of the page that constitutes one single piece of functionality, such as a map, or a set of headlines. 

> **Note** -
> An **article** element can have different **sections**, and a **section** can include different **articles**. It all depends on the structure and content of your page.

### Aside

The `<aside>` element is used to define content that is not directly related to the main content but can provide additional information, such as related links, or similar articles.

```html
<aside>
	<h2>Did you know?</h2>
	<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
</aside>
```

### Footer

```html
<footer>
	<p class="center">Copyright</p>
</footer>
```

### div

In situations where you simply want to group together elements without any specific meaning, you can use the `<div>` tag.

```html
<div>
  <h1>some title</h1>
  <p>some text</p>
  <a href="#">some link</a>
</div>
```
