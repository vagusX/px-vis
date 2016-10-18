# px-toggle-design

Toggle is a simple on/off switch. It's created with CSS applied to a checkbox and label. Use it to create simple UI elements that enable and disable things.

**px-toggle-design is a Predix UI CSS module.** You can find a demonstration and full documentation on the [Predix UI catalog](https://predixdev.github.io/predix-ui/?show=px-toggle-design&type=css]).

------------------

## Install the module

To use the toggle module, you need to install it in your project using Bower. Run this task on the command line from inside your project folder:

```
bower install --save px-toggle-design
```

------------------

## Import it in your Sass

The toggle module won't do anything until you import and configure it in your project Sass file. Follow these steps to import it:

### 1. Enable Flags

You can turn on flags to generate additional styles defined in the toggle module. To generate new styles, set any of these flags to true above the module's @import statement in your project Sass file:

```
$inuit-enable-toggle--small : true;
$inuit-enable-toggle--large : true;
$inuit-enable-toggle--huge  : true;
```

### 2. Customize Styles

You can change style variables to customize the design of the toggle module. To change styles, set any the variables below to a new value above the module's @import statement in your project Sass file:

```
$inuit-toggle-namespace
$inuit-toggle-color
$inuit-toggle-switch
$inuit-toggle-switch-border
$inuit-toggle-switch-shadow
$inuit-toggle-background
$inuit-toggle-border
$inuit-toggle-background--on
$inuit-toggle-border--on
```

### 3. Import Sass File

Import the module by placing this code into the **Objects** layer of your project Sass file:

```
@import "px-toggle-design/_objects.toggle.scss";
```

------------------

## Use it in your HTML

Toggles are just fancy checkboxes. After you import the toggle library, you can add classes to an `<input>` tag and `<label>` tag to create your toggle element.

You can create a toggle with the following code:

```
<!-- HTML and CSS get the job done, no JavaScript required -->
<input id="simpleToggle" class="toggle__input" type="checkbox">
<label for="simpleToggle" class="toggle__label"></label>
```

### Important things to remember

#### Order matters (input before label)

Your `<input>` tag must come right before you `<label>` tag, exactly as the code appears in the example above. The toggle relies on CSS's adjacent sibling selector. If you don't place the tags in the right order, the toggle won't work.

#### Match your input id and label for

Your id attribute on your `<input>` tag should match the for attribute on your `<label>` tag to keep them in sync:

```
<!-- Input and label must have the same ID -->
<input id="SAME_VALUE" class="toggle__input" type="checkbox">
<label for="SAME_VALUE" class="toggle__label"></label>
```

#### Keep classes in sync

Both the `<input>` and `<label>` tags should have the same modifiers as their sibling. For example, if you're using a small toggle, make sure you apply the `toggle__input--small` class and the `toggle__label--small` class like the example below:

```
<!-- Small modifier on both input and label -->
<input id="toggle3" class="toggle__input toggle__input--small" type="checkbox">
<label for="toggle3" class="toggle__label toggle__label--small"></label>
```

### All the possible toggles

Here are all the possible toggles you could use. Remember, you'll need to set the correct flags before importing the toggle module (see instructions above):

```
<!-- Small toggle -->
<input id="small" class="toggle__input toggle__input--small" type="checkbox">
<label for="small" class="toggle__label toggle__label--small"></label>

<!-- Regular toggle -->
<input id="regular" class="toggle__input" type="checkbox">
<label for="regular" class="toggle__label"></label>

<!-- Large toggle -->
<input id="large" class="toggle__input toggle__input--large" type="checkbox">
<label for="large" class="toggle__label toggle__label--large"></label>

<!-- Huge toggle -->
<input id="huge" class="toggle__input toggle__input--huge" type="checkbox">
<label for="huge" class="toggle__label toggle__label--huge"></label>
```

------------------

## Dependencies
This module depends on the following modules (automatically included with Bower install):

* [px-colors-design](https://github.com/PredixDev/px-colors-design)
* [px-defaults-design](https://github.com/PredixDev/px-defaults-design)
* [px-helpers-design](https://github.com/PredixDev/px-helpers-design)
