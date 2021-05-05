# Presentation Readme

## Steps to getting the markdown so Reveal.js can use it:

1. Get the markdown cleaned up
2. Create a new file from the original markdown and add _pres. So romans.md becomes romans_pres.md
3. Create the appropriate breaks in the pages:
   1. Three empy lines creates a new horizontal page (normal use)
   2. Two empy lines creates a virticle page (optional pages to present)

2. 

# Cheat Sheet

### For advancing points within a slide (add this to the end of the line):

 <!-- .element: class="fragment" -->
<!-- .element: class="fragment" data-fragment-index="26"-->
### For adding a background image:

<!-- .slide:  data-background-image="markdown/img/mount.png"  --> 

### for adding auto-animate 

<!-- .slide: data-auto-animate="" -->

### These are more options for .slide 

```html
data-background-color="aquamarine"
```

Use this to make the font as large as possible to fit in the screen:

```html
class="r-fit-text"
```
set color font etc
```
style="color:white"
```

<!-- .slide: data-background-image="https://johnwry.github.io/dm2/markdown/Romanos/img/scroll.png" data-background-size="300px" data-background-position="left" data-background-opacity="0.5"-->

```
data-background-position="right 25% bottom 25%"
```

# PANDOC
pandoc -f docx "Haciendo Hacedores de Discípulos Maestro.docx" -t markdown --wrap=none --markdown-headings=atx --extract-media=extracted-media -o discipulado2.md

# Steps to convert Word to Markdown
1. Convert using pandoc (command above)
2. Clean up markdown

	a. make sure headers (# to ######) are in place
	b. find/replace the following:
		```
		"]{.ul}**" to "</u>__"
		```
		and 
		```
		"**[" to "__<u>"
		```

