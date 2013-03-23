# The Sass Style Guide

Here are some rules to help keep your Sass maintainable while keeping
your resulting CSS performant in the browser.

You can generate a PDF or an HTML copy of this guide using
[Transmuter](https://github.com/TechnoGate/transmuter).

## Table of Contents
* [A Primer from the Sass Way](#a-primer-from-the-sass-way)
* [Cleanup Rules](#cleanup-rules)
* [Classes](#classes)
* [Variables](#variables)
* [Nesting](#nesting)
* [Functions](#functions)
* [Compass](#compass)
* [Includes](#includes)
* [Extends](#extends)
* [Mixins](#mixins)
* [Partials](#partials)

## A Primer from the Sass Way

* While there are lessons we've learned in the trenches, start with [this guide from the Sass way](http://thesassway.com/articles/sass-doesnt-create-bad-code-bad-coders-do)

## Cleanup Rules

* If you find Sass that violates any the rules in this style guide while completing your story:
  * don’t do if behind on sprint or points for that story
  * limit yourself to 30 mins - 1 hour

## Classes

* snake_case everything!  Not **CamelCase**.  Not **lowerCameCase**. Not **wHat_EVerThis_is**.  Just snake_case.
* Don't use alignment and markup based classes.
  * ex: ``.right{ float: right }``
* Tend towards verbose class names
* Better to style on class than element or id

## Variables

* Establish a base files for:
  * _sizes.scss with base variables for grid units & font sizes
  * _colors.scss with the colors from your styleguide.
* ONLY use the established variables from _sizes.scss for padding, margins, layouts, font sizes, colors, etc.
  * If you need a new color, you probably don't.
  * If you ACTUALLY need a new color, update the base _colors.scss first and use the variable from there.

## Nesting

* [Beware of inception style selectors.](http://thesassway.com/beginner/the-inception-rule)  
* In short, don't mirror your nested selectors to mirror your markup's nesting.

## Functions

* TBD

## Compass

* [Use it!](http://compass-style.org/)  When you do you'll want to keep the following things in mind:
  * Use the [rhytym](http://compass-style.org/reference/compass/typography/vertical_rhythm/#mixin-rhythm) function to establish consistency for your:
    * margin-top
    * padding-top
    * padding-bottom
    * margin-bottom
    * [Follow the setup instructions](http://compass-style.org/reference/compass/typography/vertical_rhythm/)
  * Use the [border-radius](http://compass-style.org/reference/compass/css3/border_radius/#mixin-border-radius)
  * TDB

## Includes

* TDB...but use them!

## Extends

* Never extend something that is already using an @extend
* If using extend on selection deep on page or more than 4 or 5 times on the site, create a mixin
* TBD

## Mixins

* Always use the mixins if they exist
* Never put an @extend in a mixin
* If use mixin and then often have to override something, consider adding a variable to a mixin.
* TBD

## Partials

* Paritals should be contained in a div with a class that's the name of the partial
  * ex: ``_payment_items.haml`` should have ``.payment_items`` on line #1
