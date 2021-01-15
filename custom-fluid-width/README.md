# Observable Example: Custom Fluid Width

See it live: https://observablehq.github.io/examples/custom-fluid-width/

Using the Runtime API in vanilla JavaScript to embed a notebook, the container will resize to fit the content. Sometimes we instead want the content to fit the container, e.g. where the container size is specified by CSS. We can accomplish this by overriding the `width` variable in the standard library. In this example we create a library in which `width` is defined as a [Generator](https://observablehq.com/@observablehq/introduction-to-generators) that listens for window `resize` events and yields a new value if the `clientWidth` of the container has changed.
