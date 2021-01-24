## Universal Résumé Template

## Inspiration
This was inspired by, and parts adapted from, WebPraktikos' `universal resume`, which tries harder to be supported across use cases so in case you need A4 sizing or anything else like that, I would check out his repo. 

## How to run it

<hr>

Navigate to the base directory:

```
cd resume
```

Install the dependencies:

```
npm install
```

Start the development server:

```
npm run serve
```

Only generate CSS that is used on the page which results in a much smaller file size:

```
npm run build
```

<hr>

## Starting Point

`docs/index.html` is the main content file. By copying HTML: add pages, sections, subsection, and other parts.

`npm run build` will make the **docs** directory ready for drag-n-drop to, for example, https://app.netlify.com/drop (free registration required beforehand).


<hr>

## Tailwind CSS

A nice bootstrap alternative that doesn't have as much opinionation that is all the rage these days with the 'hates css' crowd that while not a part of, I definitely didn't want to fall behind and thus I took this oppurtunity to practice a bit. 

<hr>


## Custom CSS

Code from `tailwind.config.js` and `tailwind.css` transpiles to `docs/style.css`.

<hr/>

## Balanced Columns

Removing `col-fill-auto` class will make both columns equally tall. Moreover, removing `md:h-letter` and `md:h-letter-col` classes will eliminate fixed proportions of the letter or A4 page — thereby removing unnecessary vertical space when displaying short columns.

<hr/>


## Printing

### Chrome

Right-click → Print.  
Also, choose the **Save as PDF** option if needed.

### Firefox

File → Print.

### Adobe Acrobat Reader

File → Print.

By clicking on the **Page Setup** button, you are taken to the window with A4 and Letter options.



