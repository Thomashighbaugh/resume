## Universal Résumé Template

## Inspiration
This was inspired by, and parts adapted from, WebPraktikos' `universal resume template`, which tries harder to be supported across use cases so in case you need A4 sizing or anything else like that, I would check out his repo. 

### Right to Copy or Adapt to Your Needs

This is my personal resume, written out using `universal resume template` as a guide but constitutes a distinct work product from the original and is composed using styles and font-families that constitute my personal branding, so please change at least that much if you opt to adapt it yourself, other than that, have fun and good luck with finding your next job.

<hr>

## How to run it
Clone the git repository 
```
git clone https://github.com/Thomashighbaugh/resume
```

Navigate to the base directory:

```
cd resume
```

Install the dependencies:

```
yarn install
```

Start the development server after building the stylesheet out of the Tailwind configuration:

```
yarn build && yarn serve
```

Only generate CSS that is used on the page which results in a much smaller file size:

```
yarn build
```

<hr>

## Starting Point

`docs/index.html` is the main content file. By copying HTML: add pages, sections, subsection, and other parts.

`npm run build` enables drag and drop support of the `docs` directory, which you find helpful unloading your copy on GitHub if terminal/command prompt is not your thing. 

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



