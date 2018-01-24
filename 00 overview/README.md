# Overview
Let's be very clear about the *main* reason you are considering about either of these:

1. You have data (need a lib for this)
2. You have UI that shows this data (need a lib for this) and allows the user to change this data (need a lib for this)
3. When data changes you want the UI to change (need a lib for this).

Both Angular and React can fill in this _you need a lib for this_ gap in your UI development process. How they do them is fundamentally different.

## What react with mobx does
A very simple and effective mental model to have: 

* Fundamentally you have functions (components) that map your data (mobx observables) to plain JavaScript objects (called VNodes) that you hand over to react and ask it to render to a particular mount point in the browser DOM. 
* Whenever there is a change in your data that impacts your last returned VDOM (mobx will track this for you), mobx will ask React to re-request the new `VNodes`. 
* React will take these new `VNodes`, diff them to the previous `VNodes` and apply changes in VNodes to the actual DOM it has rendered before. 

## What angular does

* You create templates and classes (components) that attach logic to these templates 
* Whenever there is a change in the data controlled by an instance of the component class changes, angular will re-render the template portions that need updating intelligently.