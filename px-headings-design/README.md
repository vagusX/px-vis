# px-headings-design

Headings gives you base-level heading sizes in the form of easy-to-apply classes. Use its classes to style H1-H6 heading tags or other text elements. This module is a fork of the [inuitcss Headings module](https://github.com/inuitcss/base.headings).

**px-headings-design is a Predix UI CSS module.** You can find a demonstration and full documentation on the [Predix UI catalog](https://predixdev.github.io/predix-ui/?show=px-headings-design&type=css]).

## Install the module

To use the headings module, you need to install it in your project using Bower. Run this task on the command line from inside your project folder:

```
bower install --save px-headings-design
```

## Import it in your Sass

The headings module won't do anything until you import and configure it in your project Sass file. Follow these steps to import it:

### 1. Enable Flags

There are no flags to set before importing this module in your project Sass file.

### 2. Customize Styles

You can change style variables to customize the design of the headings module. To change styles, set any the variables below to a new value above the module's @import statement in your project Sass file:

```
$inuit-headings-namespace
$inuit-heading-size-1
$inuit-heading-size-2
$inuit-heading-size-3
$inuit-heading-size-4
$inuit-heading-size-5
```

### 3. Import Sass File

Import the module by placing this code into the **Base** layer of your project Sass file:

```
@import "px-headings-design/_base.headings.scss";
```

## Use it in your HTML

The headings module exposes classes that set the sizes of your heading tags. Each heading size (`<h1>...</h1>` through `<h6>...</h6>`) has corresponding class listed below. Apply the class to your heading tag and the sizing will automatically happen.

```
<h4 class="epsilon">For example, here's an `h4` tag.</h4>
```

You can also apply the headings classes to non-heading tags. For example:

```
<p class="zeta">This paragraph tag can be styled like an `h6`</p>
```

(Note: There's a good accessibility case for doing this. Heading tags have meaning for screen readers and web scrapers, and you should avoid having multiple high-level heading tags that are only used for styling.)

### All the possible headings

Here are all the heading classes available:

```
<!-- Heading Size 1 -->
<h1 class="alpha">...</h1>

<!-- Heading Size 2 -->
<h2 class="beta">...</h2>

<!-- Heading Size 3 -->
<h3 class="gamma">...</h3>

<!-- Heading Size 4 -->
<h4 class="delta">...</h4>

<!-- Heading Size 5 -->
<h5 class="epsilon">...</h5>

<!-- Heading Size 6 -->
<h6 class="zeta">...</h6>
```

## Dependencies

This module depends on the following modules (automatically included with Bower install):

* [px-defaults-design](https://github.com/PredixDev/px-defaults-design)
* [px-mixins-design](https://github.com/PredixDev/px-mixins-design)
