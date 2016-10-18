# px-functions-design

The functions module contains contains functions that are required for using all Predix UI CSS modules. Use it to convert between units (i.e. pixels to REM and back again) and compute numbers.

**px-functions-design is a Predix UI CSS module.** You can find a demonstration and full documentation on the [Predix UI catalog](https://predixdev.github.io/predix-ui/?show=px-functions-design&type=css]).

## Install the module

To use the module, you need to install it in your project using Bower. Run this task on the command line from inside your project folder:

```
bower install --save px-functions-design
```

## Import it in your Sass

The module won't do anything until you import and configure it in your project Sass file. Follow these steps to import it:

### 1. Enable Flags

There are no flags to set before importing this module in your project Sass file.

### 2. Customize Styles

There are no style variables to set before importing this module in your project Sass file.

### 3. Import Sass File

Import the module by placing this code into the **Tools** layer of your project Sass file:

```
@import 'px-functions-design/_tools.functions.scss';
```

## Use it in your project

You can use this module's functions in your Sass files.

### Converting between size units

The two most-used functions provided by the functions module help convert between pixel (an absolute-size unit) and REM (a relative-size unit).

#### From pixel to REM

The `calculateRem` function takes a value in pixels and returns the equivalent in REM. You can use it like this:

```
.special-font-class {
  font-size: calculateRem(16px);
}
```

The size returned will depend on the base rem size set in your project (you'll set your base rem when you import the `px-defaults-design` module.)

#### From REM to pixel

The `remTopx` function does the opposite: it takes a value in REM and returns the equivalent in pixels. You can use it like this:

```
.another-special-font-class {
  font-size: remToPx(1.4rem);
}
```

Again, the size returned will depend on the base rem size set in your project.

## Additional functions

The functions module also provides a set of related utilities that take a number and compute a multiple or fraction of it. For example, you can use the following function to get the result of 3 * 4 and convert it to REM.

```
.big-font-class {
  // Multiplying by 1rem is a simple way to add units after doing math
  font-size: triple(3) * 1rem;
}
```

In addition to `triple`, you can use `quarter`, `halve`, `double`, `quadruple`, and `third`. All functions will return rounded integers.

## Dependencies

This module depends on the following modules (automatically included with Bower install):

* [px-defaults-design](https://github.com/PredixDev/px-defaults-design)
* [inuit-functions](https://github.com/inuitcss/tools.functions)
