# TODO: 
* ng-click

# Abstract chores
## Conditional display 
* React : use `&&`. OR `?:` or `if else`
* Angular : use `ng-if`
  * Worth mentioning that it is very common to see miss the fact that some item is *visible or not* because the `ng-if` gets hidden as it is not the *start* of the statement. (compare `if (foo) div` vs. `div if(foo)`)

## Choose between multiple views
* React: use `switch` 
* Angular: ng-switch


## For loop 
* React: use `.map` on your arrays
* ng-for

## Global Handlers 
* React use `addEventListener` / `removeEventListener`
* Angular : Use angular specific apis. [ref](https://stackoverflow.com/questions/36123380/global-events-window-onresize-didnt-change-the-local-variables-value/36135449#36135449)

## Intellisense 
* React: Built into TypeScript.
* Angular: Seperate plugin by the angular team.

## Formatters 
pipes (Just use JavaScript functions that are completely independent of framework)

## HTML Reuse
* Here is a piece of HTML that you need to duplicate. Do it in React, Do it in Angular

## Transclusion 
* Just pass VNodes around instead of lots of framework code.
* Multi-slot Transclusion : Just adding more concepts without much value.

