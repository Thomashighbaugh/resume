## Universal Résumé Template

## What This Is

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

## 🚀 Recent Upgrade: Tailwind CSS v3.4.19

This resume has been successfully upgraded from Tailwind CSS v3.3.5 to v3.4.19 with significant enhancements:

### 📈 What's New

**Tailwind CSS Upgrade:**
- ✅ Upgraded from v3.3.5 → v3.4.19 (latest stable v3.x)
- ✅ All dependencies updated for better performance and security
- ✅ Build size optimized (24.5KB → 13.1KB) with improved PurgeCSS
- ✅ Full backward compatibility maintained

**Enhanced Responsive Design:**
- 🎯 **2K Support**: Custom `2xl` breakpoint at 1440px
- 🎯 **4K Support**: Custom `4xl` breakpoint at 2160px  
- 🎯 **Height Utilities**: Viewport-based height classes for better responsive control
- 🎯 **Typography Scaling**: Automatic text scaling for high-resolution displays

**Developer Experience:**
- ⚡ Faster builds with optimized content configuration
- 🔧 Better PostCSS integration with latest plugins
- 📦 Cleaner dependency tree with updated packages
- 🛡️ Enhanced security with latest dependency versions

### 📱 Responsive Breakpoints

| Breakpoint | Min-Width | Target Display |
|------------|-----------|----------------|
| `xsm` | 500px | Large phones |
| `sm` | 640px | Small tablets |
| `md` | 833px | Tablets |
| `lg` | 1079.5px | Laptops |
| `xl` | 1280px | Desktops |
| `2xl` | 1440px | 2K displays |
| `4xl` | 2160px | 4K displays |

### 🎨 Visual Improvements

**On 2K Displays (1440px+):**
- Larger typography for better readability
- Increased padding and spacing
- Wider content containers (max-width: 6xl)
- Enhanced column gaps

**On 4K Displays (2160px+):**
- Maximum typography scaling
- Generous padding and spacing  
- Ultra-wide containers (max-width: 7xl)
- Optimal column spacing for large screens

**All Screen Sizes:**
- No visual regression on smaller screens
- Maintained print optimization
- Consistent brand presentation
- Improved readability across all devices

<hr>

## Starting Point

`docs/index.html` is the main content file. By copying HTML: add pages, sections, subsection, and other parts.

`npm run build` enables drag and drop support of the `docs` directory, which you find helpful unloading your copy on GitHub if terminal/command prompt is not your thing. 

<hr>

## Tailwind CSS

A nice bootstrap alternative that doesn't have as much opinionation that is all the rage these days with the 'hates css' crowd that while not a part of, I definitely didn't want to fall behind and thus I took this oppurtunity to practice a bit. 

**Recently Upgraded:** This project now uses **Tailwind CSS v3.4.19** (latest stable v3.x) with enhanced responsive capabilities including **2K and 4K display support**.

### 📱 Enhanced Responsive Design

The resume now includes custom breakpoints optimized for high-resolution displays:

- **2xl (2K)**: `1440px` - For 1440p displays and large laptops
- **4xl (4K)**: `2160px` - For 4K monitors and high-DPI displays

### ✨ New Responsive Features

**Typography Scaling:**
- Larger, more readable text on 2K+ displays
- Name scales from `5xl` → `6xl` (2K) → `7xl` (4K)
- Job title scales from `2xl` → `3xl` (2K) → `4xl` (4K)
- Body text automatically scales with viewport

**Layout Improvements:**
- Increased padding and spacing on large displays
- Wider max-width containers for better use of screen real estate
- Enhanced column gaps for improved readability
- Optimized initials block sizing

**Height-Responsive Utilities:**
- `screen-75`, `screen-80`, `screen-90`, `screen-95` for viewport-based heights
- Matching `min-height` and `max-height` utilities
- Perfect for responsive modals and sections

### 🎯 Usage Examples

**2K Display Optimizations:**
```html
<div class="p-16 2xl:p-20 text-2xl 2xl:text-3xl">
  Enhanced for 2K displays
</div>
```

**4K Display Optimizations:**
```html
<h1 class="text-5xl 2xl:text-6xl 4xl:text-7xl">
  Scales beautifully across all displays
</h1>
```

**Height-Responsive Design:**
```html
<section class="min-h-screen-75 max-h-screen-90">
  Responsive to viewport height
</section>
```

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

OR 

You can save it as a PDF which will probably keep the SVG image and the other things being stripped out by the print optimizations, but there are use cases for that as well and its not like there really is a `right way` 

------

### Firefox

File → Print.

### Adobe Acrobat Reader

File → Print.

By clicking on the **Page Setup** button, you are taken to the window with A4 and Letter options.



