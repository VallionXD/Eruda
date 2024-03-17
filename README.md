# Eruda
> Original by liriliri, this is just a backup incase it ever goes down. And this repository has compiled plugin scripts. Everything in here but this message is from liriliri's readme.

Amazing mobile inspect element from a bookmark, made by liriliri.

## Bookmark
> You can use this bookmark to access eruda any time with the click of a button.

```js
javascript:(function () { var script = document.createElement('script'); script.src="https://cdn.jsdelivr.net/npm/eruda"; document.body.append(script); script.onload = function () { eruda.init(); } })();
```

**Script Source:** [https://cdn.jsdelivr.net/npm/eruda](https://cdn.jsdelivr.net/npm/eruda)

## Configuration

When initialization, a configuration object can be passed in.

* container: Container element. If not set, it will append an element directly
under html root element.
* tool: Choose which default tools you want, by default all will be added.

For more information, please check the [documentation](doc/API.md).

```javascript
let el = document.createElement('div');
document.body.appendChild(el);

eruda.init({
    container: el,
    tool: ['console', 'elements']
});
```

## Plugins

* [eruda-monitor](https://github.com/liriliri/eruda-monitor): Display page fps and memory.
* [eruda-features](https://github.com/liriliri/eruda-features): Browser feature detections.
* [eruda-timing](https://github.com/liriliri/eruda-timing): Show performance and resource timing.
* [eruda-code](https://github.com/liriliri/eruda-code): Run JavaScript code.
* [eruda-benchmark](https://github.com/liriliri/eruda-benchmark): Run JavaScript benchmarks.
* [eruda-geolocation](https://github.com/liriliri/eruda-geolocation): Test geolocation.
* [eruda-orientation](https://github.com/liriliri/eruda-orientation): Test orientation api.
* [eruda-touches](https://github.com/liriliri/eruda-touches): Visualize screen touches.

If you want to create a plugin yourself, follow the guides [here](./doc/PLUGIN.md).

## Related Projects

* [eruda-android](https://github.com/liriliri/eruda-android): Simple webview with eruda loaded automatically.
* [chii](https://github.com/liriliri/chii): Remote debugging tool.
* [chobitsu](https://github.com/liriliri/chobitsu): Chrome devtools protocol JavaScript implementation.
* [licia](https://github.com/liriliri/licia): Utility library used by eruda.
* [luna](https://github.com/liriliri/luna): UI components used by eruda.
* [vivy](https://github.com/liriliri/vivy-docs): Banner image generation.

## Third Party

* [eruda-pixel](https://github.com/Faithree/eruda-pixel): UI pixel restoration tool.
* [eruda-webpack-plugin](https://github.com/huruji/eruda-webpack-plugin): Eruda webpack plugin.

## Original

[Original Repository Here..](https://github.com/liriliri/eruda/)

### License

See liriliri's license, as I do not own this software.

[Liriliri's License Here..](https://github.com/liriliri/eruda/blob/master/LICENSE)
