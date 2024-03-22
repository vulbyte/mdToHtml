# mdToHtml

a simple md to html converter. why? because i want to without relying on a random npm package

## goal:

to make a simple js file that you can call with 1 simple input, which is the file,
and will easily return html elements.

### example:

```
input:
example.md
|
| # title
| text
|
| <br/>
|
| ## title 2
| more text
|
| <br/>
|
| _italic text_
| _more italic text_
|
| <br/>
|
| **bold text**
| **moar bold text**
|
| <br/>
|
| [link name](external_link)
|
| <br/>
|
| 1. ol 1
| 1. ol 2
| 1. ol 3
|
| <br/>
|
| - ul 1
| - ul 2
| - ul 3
|
| <br/>
|
| ---
| \*\*\*
|
| <br/>
|
| `code`
|
| <br/>
|
| [image](image.png)
```

output:

```
<div class="convertedMd">
    <h1> title </h1>
    <p> text </p>
    <br/>
    <h2> title 2 </h2>
    <p> more text </p>
    <br/>
    <i> italic text </i>
    <i>_more italic text_</i>
    <br/>
    <b> bold text </b>
    <b> moar bold text </b>
    <br/>
    <a href="external_link"> link name </a>
    <br/>
    <ol>
        <li> ol 1 </li>
        <li> ol 2 </li>
        <li> ol 3 </li>
    </ol>
    <br/>
    <ul>
        <li> ul 1 </li>
        <li> ul 2 </li>
        <li> ul 3 </li>
    </ul>
    <br/>
    <hr/>
    <hr/>
    <code> code </code>
    <br/>
    <img src="image.png" alt=image />
</div>
```
