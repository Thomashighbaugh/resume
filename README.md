## Universal Résumé Template

## WHat This Is

This is the repository housing my personal resume, which I can conveniently host as a website because instead of writing it in Word (which I can't do as a Linux user) or Libreoffice (which sucks) or LaTex (which I have done, but is a bit of a pain and OverLeaf is a challenge itself) I opted to **write it out in HTML**. 

There is really no reason I have come across that I shouldn't use **HTML** to write my resume, since I know it pretty well and write a lot of notes and documents in it or at least **MArkdown** that is just a shorthand of **HTML** anyway. It is easy to write, most code editors can syntax highlight it without need for additional modifications (including some included text editors for various desktop environments) and its a lot more powerful than using the same 5 word templates over and over again. I want to show people that may hire me something unique, so here it is. 

## Inspiration
This was inspired by, and parts adapted from, WebPraktikos' `universal resume template`, which tries harder to be supported across use cases so in case you need A4 sizing or anything else like that, I would check out his repo. I cannot understate how enlightening I found that project and how deeply it inspired this one. 

Additional props goes to the author of [heropatterns](https://heropatterns.com) who provided the svg pattern I have gotten somewhat experimental with as the background. **SVG** is essentially **HTML** with some unique tags called paths, so its pretty natural I would use something like that in this resume, but it would have probably taken me decades to come up with some of the awesome patterns you can use free of charge thanks to **heropatterns** which is pretty awesome and definitely worth looking into to give your site a little `sugar`. 

### Right to Copy or Adapt to Your Needs

This is my personal resume, written out using `universal resume template` as a guide, which means my name and information is all over the thing and I didn't set it up specifically to be a template or anything, so I would advise if you use it yourself, probably best to change the name and contact information (but if not and you get me a job, I really wouldn't mind!). Other than that, have fun and good luck with finding your next job. The beauty of open source my friends, I borrow from you and you borrow from me and we all are better for it. 

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

**Note:** The way I am using Tailwind here varies wildly from the way I use it elsewhere and is a bit of an old school way to deploy it but `it works` just fine so I am not going to throw the monkey wrench in the project anytime soon on that front. 

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



