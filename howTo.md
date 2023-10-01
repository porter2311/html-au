# How To

## If you already know custom elements

1. Assuming you use some bundling technology like rollup, Webpack, or Vite. When you import the auObserver into app.js everything else is taken care of.
1. create a custom element and register it in the browser. Nothing AU-specific in this step.
1. Set up the auObserver to observe document.body or a root element in your application or component.
1. start with something a user would click on like a div or a button
1. add the au- attributes to the element. 
1. add the name of the component to au-post or au-get for example au-get="component name"
1. add the au-target="CSS selector of the target" - where you want the component to appear on the dom
1. when the user clicks on your div

### Passing data to the custom element

Works similarly to a good old fashioned forms example from 1995, but with a twist.
But instead of the FormData being sent to the server it is sent to the component.
The data will magically appear as a model in your component. Or 'body' if you want the raw FormData.
But you need to ensure that your component defines 'model' or 'body'. If not nothing will be passed to it.

## If you do not already know custom elements

