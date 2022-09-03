# Geany HTML Snippets

## Introduction

I was a fan of [Notepad++](https://notepad-plus-plus.org/) source code editor, but it doesn't support Linux Operating System. Since I'm also a fan of Linux, so I decided to switch to another lightweight text editor. 

Fortunately, I found [Geany](https://www.geany.org/), a powerful, stable and lightweight programmer's text editor that provides tons of useful features without bogging down your workflow. It runs on Linux, Windows and macOS is translated into over 40 languages, and has built-in support for more than 50 programming languages.

However, Geany doesn't have [Emmet](https://emmet.io/) plugin for now. So for speeding up the workflow of my daily web development, I decided to make my version of HTML snippets for Geany. And I made it, it's not perfect but "as long as it's simple, it makes your life simple". For those who want to use it as your HTML snippets in Geany, I made an instruction below for you guys on how to add snippets into Geany.

## Getting Started

> ### Step 1: Copy the example snippets from below or snippets.conf

```
[HTML]
# HTML 5 Template
html5=<!DOCTYPE html>\n<html lang="en">\n<head>\n\t<meta charset="UTF-8">\n\t<meta http-equiv="X-UA-Compatible" content="IE=edge">\n\t<meta name="viewport" content="width=device-width, initial-scale=1.0">\n\t<title>%cursor%</title>\n</head>\n<body>\n\t\n</body>\n</html>
# HTML Basic
doctype=<!DOCTYPE html>
html=<html lang="en">%cursor%</html>
body=<body>%cursor%</body>
# HTML Headings
h1=<h1>%cursor%</h1>
h2=<h2>%cursor%</h2>
h3=<h3>%cursor$</h3>
h4=<h4>%cursor%</h4>
h5=<h5>%cursor%</h5>
h6=<h6>%cursor%</h6>
# HTML Paragraphs
p=<p>%cursor%</p>
hr=<hr>
br=<br>
pre=<pre>%cursor%</pre>
# HTML Formatting
b=<b>%cursor%</b>
strong=<strong>%cursor%</strong>
i=<i>%cursor%</i>
em=<em>%cursor%</em>
mark=<mark>%cursor%</mark>
small=<small>%cursor%</small>
del=<del>%cursor%</del>
ins=<ins>%cursor%</ins>
sub=<sub>%cursor%</sub>
sup=<sup>%cursor%</sup>
# HTML Quotations
blockquote=<blockquote>%cursor%</blockquote>
blockquotecite=<blockquote cite="">%cursor%</blockquote>
q=<q>%cursor%</q>
abbr=<abbr title="">%cursor%</abbr>
address=<address>%cursor%</address>
cite=<cite>%cursor%</cite>
bdo=<bdo dir="rtl">%cursor%</bdo>
# HTML CSS
style=<style>%cursor%</style>
link=<link rel="stylesheet" href="%cursor%">
# HTML Links
a=<a href="">%cursor%</a>
atarget=<a href="" target="">%cursor%</a>
# HTML Images
img=<img src="%cursor%" alt="">
map=<map name="%cursor%"></map>
area=<area shape="" coords="" alt="" href="%cursor%">
picture=<picture>%cursor%</picture>
sourcemedia=<source media="(min-width:)" srcset="%cursor%">
# HTML Favicon
linkicon=<link rel="icon" type="image/x-icon" href="%cursor%">
# HTML Tables
table=<table>%cursor%</table>
th=<th>%cursor%</th>
tr=<tr>%cursor%</tr>
td=<td>%cursor%</td>
caption=<caption>%cursor%</caption>
colgroup=<colgroup>%cursor%</colgroup>
col=<col>%cursor%</col>
thead=<thead>%cursor%</thead>
tbody=<tbody>%cursor%</tbody>
tfoot=<tfoot>%cursor%</tfoot>
# HTML Lists
ul=<ul>%cursor%</ul>
ol=<ol type="">%cursor%</ol>
li=<li>%cursor%</li>
dl=<dl>%cursor%</dl>
dt=<dt>%cursor%</dt>
dd=<dd>%cursor%</dd>
# HTML Block & Inline
div=<div>%cursor%</div>
span=<span>%cursor%</span>
# HTML Iframes
iframe=<iframe src="%cursor%" width="" height=""></iframe>
# HTML JavaScript
script=<script>%cursor%</script>
scriptsrc=<script src="%cursor%"></script>
noscript=<noscript>%cursor%</noscript>
# HTML Head
head=<head>%cursor%</head>
title=<title>%cursor%</title>
meta=<meta name="%cursor%" content="">
metacharset=<meta charset="UTF-8">
metahttp=<meta http-equiv="X-UA-Compatible" content="IE=edge">
metaviewport=<meta name="viewport" content="width=device-width, initial-scale=1.0">
base=<base href="%cursor%">
basetarget=<base href="%cursor%" target="">
# HTML Layout
header=<header>%cursor%</header>
nav=<nav>%cursor%</nav>
section=<section>%cursor%</section>
article=<article>%cursor%</article>
aside=<aside>%cursor%</aside>
footer=<footer>%cursor%</footer>
details=<detials>%cursor%</details>
summary=<summary>%cursor%</summary>
# HTML Computer Code
kbd=<kbd>%cursor%</kbd>
samp=<samp>%cursor%</samp>
code=<code>%cursor%</code>
var=<var>%cursor%</var>
# HTML Semantics
figure=<figure>%cursor%</figure>
figcaption=<figcaption>%cursor%</figcaption>
main=<main>%cursor%</main>
time=<time datetime="">%cursor%</time>
# HTML Forms
form=<form action="" method="%cursor%"></form>
formenctype=<form action="" method="post" enctype="multipart/form-data">%cursor%</form>
input=<input type="%cursor%">
label=<label for="%cursor%"></label>
select=<select>%cursor%</select>
option=<option value="">%cursor%</option>
textarea=<textarea rows="%cursor%" cols=""></textarea>
button=<button>%cursor%</button>
fieldset=<fieldset>%cursor%</fieldset>
legend=<legend>%cursor%</legend>
datalist=<datalist>%cursor%</datalist>
output=<output for="%cursor%"></output>
# HTML Canvas
canvas=<canvas>%cursor%</canvas>
# HTML SVG
sv=<svg>%cursor%</svg>
circle=<circle cx="%cursor%" cy="" r=""/>
rect=<rect width="%cursor%" height=""/>
polygon=<polygon point="%cursor%"/>
defs=<defs>%cursor%</defs>
linearGradient=<linearGradient x1="" y1="" x2="" y2="">%cursor%</linearGradient>
stop=<stop offset="%cursor%"/>
ellipse=<ellipse cx="" cy="" rx="" ry="" fill="url(%cursor%)"/>
text=<text fill="" font-size="" font-family="" x="" y="">%cursor%</text>
# HTML Video
video=<video controls>%cursor%</video>
sourcevideo=<source src="%cursor%" type="video/mp4">
track=<track src="%cursor%" kind="subtitles" srclang="" label="">
# HTML Audio
audio=<audio controls>%cursor%</audio>
sourceaudio=<source src="%cursor%" type="audio/mpeg">
# HTML Plug-ins
object=<object data="%cursor%"></object>
embed=<embed src="%cursor%">
# JavaScript
if=if(%cursor%){\n\t\n}
else=else{\n\t%cursor%\n}
for=for(%cursor%){\n\t\n}
while=while(%cursor%){\n\t\n}
do=do{\n\t%cursor%\n}while()
switch=switch(%cursor%){\n\tcase :\n\t\t\n\t\tbreak;\n\tdefault:\n\t\t\n}
try=try{\n\t%cursor%\n}catch(){\n\t\n}
```

> ### Step 2: Open Geany and go to Tools -> Configuration Files -> snippets.conf

![Step 2](./Step_2.png)

> ### Step 3: Paste to the `[HTML]` section as replacement and save it

![Step 3](./Step_3.png)

> ### Step 4: Happy coding!

## Summary

If you follow my instruction above, you will be able to use the snippets. Hope it helps you. Feel free to open issue if you have any issues. 
