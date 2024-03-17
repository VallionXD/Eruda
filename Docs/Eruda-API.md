# Eruda Documentation: API
> This is a remade version of the official docs for the api.

## Init: `eruda.init()`
> Documentation for the initialization function.

### Options
| Name | Type | Description |
| ----- | ----- | ----- |
| `container` | **element** | Container element. If this is not set, it will *automatically* append an element directly under the *html root element.* |
| `tool` | **string-array** | Choose which default tools you would like, by default all are *available*. |
| `autoScale` | **boolean** | Auto scale eruda window for different *viewport sizes* and *settings*. Defaults to *true*. |
| `useShadowDom` | **boolean** | Use shadow dom for css enscapulation. Defualts to *true*. |
| `defaults` | **object** | Default settings for eruda. |

**Available Default Strings:**

| **Name** | **Type** | **Description** |
| ----- | ----- | ----- |
| `transparency` | **number** | Eruda transparency, from *0* to *100*. |
| `displaySize` | **number** | Eruda display size, from *0* to *100*. |
| `theme` | **string** | Set the theme. *Dark* or *Light* mode defaults to browser preference.  |

#### Example Usage
> An Example of all the mentioned above.

```javascript
// Create a div container element.
const containerElement = document.createElement("div");

// Append the container element to the body.
document.body.appendChild(containerElement);

// Intitialize Eruda.
eruda.init({
  // Set the container to use.
  container: containerElement,

  // Define the tools available.
  tools: [
    "console",
    "elements"
  ],

  // Define if using shadow dom.
  useShadowDom: true,

  // Define if using autoscale.
  autoScale: true,

  // Set the defaults.
  defaults: {
    displaySize: 50,
    transparency: 0.9
    theme: "Monokai Pro"
  } 
});
```

You can also define the options, and use them like *below*.

```javascript
// Define the options.
const options = {
  // Set the container to use.
  container: containerElement,

  // Define the tools available.
  tools: [
    "console",
    "elements"
  ],

  // Define if using shadow dom.
  useShadowDom: true,

  // Define if using autoscale.
  autoScale: true,

  // Set the defaults.
  defaults: {
    displaySize: 50,
    transparency: 0.9
    theme: "Monokai Pro"
  } 
};

// Initialize Eruda.
eruda.init(options);
```

## Destroy: `eruda.destroy()`
> The function to destroy the current Eruda instance.

There isn't much to say about this feature, it is self explanitory. If you have a running instance of Eruda and you run this command it will destroy the instance.

```javascript
// Destroy the current instance of Eruda.
eruda.destroy();
```

## Scale: `eruda.scale()`
> Function to get, or set the scale of the current Eruda instance.

This feature can get or set the current Eruda instance's scale. Below is how you get the scale.

```javascript
// Get the scale of the current Eruda instance.
eruda.scale(); // --> 1
```

If you want to set the scale of the current instance, do as below.

```javascript
// Set the scale of the current Eruda instance.
eruda.scale(1.5);

// Get the scale of the current Eruda instance.
eruda.scale(); // --> 1.5
```

## Add & Remove: `eruda.add()`, `eruda.remove()`
> These functions are used to add and remove a tool from the current instance of Eruda.

The add function is used to add a tool to your current instance of Eruda. Below is an example of how it would work.

```javascript
// Add a custom tool to the current instance of eruda.
eruda.add(new (eruda.Tool.extend({
      // Set the name of the new tool.
      name: "test"
    })
  )
);

// Add the built-in network tool to the current instance of Eruda.
eruda.add(eruda.Network);
```

The remove function is used to add a tool to your current instance of Eruda. Below is an example of how it would work.

```javascript
// Remove the custom tool "Test" added in the previous example, from current instance of Eruda.
eruda.remove("test");

// Remove the built-in console tool from the current instance of Eruda.
eruda.remove("console");
```

## Show & Hide: `eruda.show()`, `eruda.hide()`
> These functions are used to show and hide the current instance of Eruda.

The show function is used to show the current instance of Eruda, below is how you do it.

```javascript
// Show the current instance of Eruda.
eruda.show();
```

The hide function is used to hide the cuirrent instance of Eruda, below is how you do it.

```javascript
// Hide the current instance of Eruda.
eruda.hide();
```
