# The Sass Style Guide

Here are some rules to help keep your Sass maintainable while keeping
your resulting CSS performant in the browser.

You can generate a PDF or an HTML copy of this guide using
[Transmuter](https://github.com/TechnoGate/transmuter).

## Table of Contents
* [A Primer from the Sass Way](#a-primer-from-the-sass-way)
* [Cleanup Rules](#cleanup-rules)
* [Classes](#classes)
* [Nesting](#nesting)
* [Compass](#compass)
* [Includes](#includes)
* [Extends](#extends)
* [Mixins](#mixins)

## A Primer from the Sass Way

* While there are lessons we've learned in the trenches, start with [this guide from the Sass way](http://thesassway.com/articles/sass-doesnt-create-bad-code-bad-coders-do)

## Cleanup Rules

* If you find Sass that violates any the rules in this style guide while completing your story:
  * don’t do if behind on sprint or points for that story
  * limit yourself to 30 mins - 1 hour

## Classes

* CamelCase everything.  Not **snake_cased_name**.  Not **lowerCameCase**. Not **wHat_EVerThis_is**.  Just CamelCase.

## Nesting

* [Beware of inception style selectors.](http://thesassway.com/beginner/the-inception-rule)  
* In short, don't mirror your nested selectors to mirror your markup's nesting.

## Compass

* [Use it!](http://compass-style.org/)  When you do you'll want to keep the following things in mind:
  * TDB

## Includes

* TDB...but use them!

## Extends

* Never extend something that is already using an @extend
* TBD

## Mixins

* TBD
