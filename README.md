# Elastic Grids

> - Fully customizable and responsive CSS Grids with Sass.
> - Give you a set of CSS helper classes for dealing with widths/proportions.
> - Only enable what you needs. Keep control on the generated CSS.


## How it works

Elastic-Grids consist of two types of helpers: 

#### Grids

The grid class `.grid`

#### Widths

Widths helpers for all needed proportions (`2/3`, `3/4`, `8/12`...).

_[More documentation coming soon...]_

## Installation

Install using Bower:

    $ bower install --save elastic-grids

Install using npm:

    $ npm install --save elastic-grids

Usage:

```scss
$elastic-grids: true;
$elastic-widths: 1, 2, 3, 4, 6, 9, 12;
  
@import "elastic-grids";
@include elastic-widths($elastic-widths);
```

By default the **Grid** helpers are not generated, until you specify `$elastic-grids: true;`.

The first parameter of `elastic-widths` corespond to the **Widths** you needs. Again you have the control of what CSS you want to generate.


## Optional Settings

Some optional settings you can specify before the import.

#### Use spoken-word selector instead of fractions

If you don't like the fraction attribute selector `<div class="1/2">`,
you can use the spoken-word format instead, e.g. `<div class="one-half">`.

```scss
$elastic-widths-use-fractions: false;
```

#### Rename the Grid class name

```scss
$elastic-grids-class-name: "grid";
```

#### Add Prefix/Suffix to the Width classes

```scss
@include elastic-widths($elastic-widths, $prefix: "u-", $suffix: "--test");
```

#### Specify a custom width selector inside a grid

```scss
$elastic-widths-custom-selector: '[class^="u-"], [class*=" u-"]';
```

## Responsive Grids and Widths

_[More documentation coming soon...]_


## Licence

Copyright (c) 2015, Etienne Magnier.<br />
Licenced under the BSD license. See the 
[LICENSE file](https://github.com/emagnier/elastic-grids/blob/master/LICENSE.md) for license text 
and copyright information.
