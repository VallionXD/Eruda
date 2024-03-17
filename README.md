[//]: # (Create a div to center the title and the image.)
<div align="center">
    <h1 align="center">Eruda</h1>
    <div style="box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5);">
        <img alt="Eruda Preview" src="https://github.com/VallionXD/Eruda/assets/151787330/64f77792-126a-4968-8869-b9525efcd1cb">
    </div>
</div>

[//]: # (Use the blank <p> tag to seperate the > after the <p> tag.)
<p></p>

> Original by liriliri, this is just a backup incase it ever goes down. And this repository has compiled plugin scripts. Everything in here but this message is from liriliri's readme.

Amazing mobile inspect element from a bookmark, made by liriliri.

## Bookmark
> You can use these bookmarks to access eruda any time with the click of a button.

### Eruda NPM [JSDelivr]
```js
javascript:(function () { var script = document.createElement('script'); script.src="https://cdn.jsdelivr.net/npm/eruda"; document.body.append(script); script.onload = function () { eruda.init(); } })();
```
**Script Source:** [https://cdn.jsdelivr.net/npm/eruda](https://cdn.jsdelivr.net/npm/eruda)

### My Repo [JSDelivr]
```js
javascript:(function () { var script = document.createElement('script'); script.src="https://cdn.jsdelivr.net/gh/VallionXD/Eruda@main/eruda.js"; document.body.append(script); script.onload = function () { eruda.init(); } })();
```
**Script Source:** [https://github.com/VallionXD/Eruda/blob/main/eruda.min.js](https://github.com/VallionXD/Eruda/blob/main/eruda.min.js)

## Installation
> Installation guide for eruda.

### NPM
> How to install eruda from the npm package.

First, install the package from npm.

```powershell
npm install eruda --save
```

Then you can add it to your webpage like so.
```html
<script src="node_modules/eruda/eruda.js"></script>
<script>eruda.init();</script>
```

## Configuration
> Adding configuration to eruda throug the init function

In the initialization, a configuration object can be passed in.

* `container`: Container element. If not set, it will append an element directly
under html root element.
* `tool`: Choose which default tools you want, by default all will be added.

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
> You can use the script below to choose which plugin to load.

```js
javascript:(function () { var script = document.createElement('script'); script.src="https://cdn.jsdelivr.net/gh/VallionXD/Eruda@main/plugins/loader.js"; document.body.append(script); script.onload = function () { eruda.init(); } })();
```

### All Plugins
> List of all the official plugins for eruda.

[//]: # (All of the plugions in a div container.)
<div>
    <details>
        <summary><b>Eruda Monitor Plugin</b></summary>
        <p><i>Display page fps and memory.</i></p>
        <ul>
            <li><a href="https://github.com/VallionXD/Eruda/plugins/blob/main/eruda-monitor.js">Plugin Link [This Repo]</a></li>
            <li><a href="https://github.com/liriliri/eruda-monitor">Plugin Link [Liriliri's Repo]</a></li>
        </ul>
    </details>
    <details>
        <summary><b>Eruda Features Plugin</b></summary>
        <p><i>Browser feature detections.</i></p>
        <ul>
            <li><a href="https://github.com/VallionXD/Eruda/plugins/blob/main/eruda-monitor.js">Plugin Link [This Repo]</a></li>
            <li><a href="https://github.com/liriliri/eruda-features">Plugin Link [Liriliri's Repo]</a></li>
        </ul>
    </details>
    <details>
        <summary><b>Eruda Timing Plugin</b></summary>
        <p><i>Show performance and resource timing.</i></p>
        <ul>
            <li><a href="https://github.com/VallionXD/Eruda/plugins/blob/main/eruda-timing.js">Plugin Link [This Repo]</a></li>
            <li><a href="https://github.com/liriliri/eruda-timing">Plugin Link [Liriliri's Repo]</a></li>
        </ul>
    </details>
    <details>
        <summary><b>Eruda Code Plugin</b></summary>
        <p><i>Run JavaScript code.</i></p>
        <ul>
            <li><a href="https://github.com/VallionXD/Eruda/plugins/blob/main/eruda-code.js">Plugin Link [This Repo]</a></li>
            <li><a href="https://github.com/liriliri/eruda-code">Plugin Link [Liriliri's Repo]</a></li>
        </ul>
    </details>
    <details>
        <summary><b>Eruda Benchmark Plugin</b></summary>
        <p><i>Run JavaScript benchmarks.</i></p>
        <ul>
            <li><a href="https://github.com/VallionXD/Eruda/plugins/blob/main/eruda-benchmark.js">Plugin Link [This Repo]</a></li>
            <li><a href="https://github.com/liriliri/eruda-benchmark">Plugin Link [Liriliri's Repo]</a></li>
        </ul>
    </details>
    <details>
        <summary><b>Eruda Geolocation Plugin</b></summary>
        <p><i>Test geolocation.</i></p>
        <ul>
            <li><a href="https://github.com/VallionXD/Eruda/plugins/blob/main/eruda-geolocation.js">Plugin Link [This Repo]</a></li>
            <li><a href="https://github.com/liriliri/eruda-geolocation">Plugin Link [Liriliri's Repo]</a></li>
        </ul>
    </details>
    <details>
        <summary><b>Eruda Orientation Plugin</b></summary>
        <p><i>Test orientation api.</i></p>
        <ul>
            <li><a href="https://github.com/VallionXD/Eruda/plugins/blob/main/eruda-orientation.js">Plugin Link [This Repo]</a></li>
            <li><a href="https://github.com/liriliri/eruda-monitor">Plugin Link [Liriliri's Repo]</a></li>
        </ul>
    </details>
    <details>
        <summary><b>Eruda Touches Plugin</b></summary>
        <p><i>Visualize screen touches.</i></p>
        <ul>
            <li><a href="https://github.com/VallionXD/Eruda/plugins/blob/main/eruda-touches.js">Plugin Link [This Repo]</a></li>
            <li><a href="https://github.com/liriliri/eruda-touches">Plugin Link [Liriliri's Repo]</a></li>
        </ul>
    </details>
</div>

### Older plugins.
> Some older plugins, that are still supported. These aren't mentioned on the official repository, although are by liriliri.

<div>
    <details>
        <summary><b>Eruda Dom Plugin</b></summary>
        <p><i>Eruda plugin for navigating dom tree.</i></p>
        <br>
        <ul>
            <li><a href="https://github.com/VallionXD/Eruda/plugins/blob/main/eruda-dom.js">Plugin Link [This Repo]</a></li>
            <li><a href="https://github.com/liriliri/eruda-dom">Plugin Link [Liriliri's Repo]</a></li>
        </ul>
    </details>
    <details>
        <summary><b>Eruda FPS Plugin</b></summary>
        <p><i>Eruda plugin for displaying fps info.</i></p>
        <ul>
            <li><a href="https://github.com/VallionXD/Eruda/plugins/blob/main/eruda-fps.js">Plugin Link [This Repo]</a></li>
            <li><a href="https://github.com/liriliri/eruda-fps">Plugin Link [Liriliri's Repo]</a></li>
        </ul>
    </details>
</div>

If you want to create a plugin yourself, follow the guides [here](./docs/PLUGIN.md)!

## Related Projects
> Plugins related to eruda mobile inspect.

* `eruda-android`: Simple webview with eruda loaded automatically. | [Link to repository](https://github.com/liriliri/eruda-android)
* `chii`: Remote debugging tool. | [Link to repository](https://github.com/liriliri/chii)
* `chobitsu`: Chrome devtools protocol JavaScript implementation. | [Link to repository](https://github.com/liriliri/chobitsu)
* `licia`: Utility library used by eruda. | [Link to repository](https://github.com/liriliri/licia)
* `luna`: UI components used by eruda. | [Link to repository](https://github.com/liriliri/luna)
* `vivy`: Banner image generation. | [Link to repository](https://github.com/liriliri/vivy-docs)

## Third Party

* `eruda-webpack-plugin`: Simple webview with eruda loaded automatically. | [Link to repository](https://github.com/liriliri/eruda-android)
* `eruda-pixel`: Remote debugging tool. | [Link to repository](https://github.com/huruji/eruda-webpack-plugin)

## Original

[Original Repository Here..](https://github.com/liriliri/eruda/)

### License

See liriliri's license, as I do not own this software.

[Liriliri's License Here..](https://github.com/liriliri/eruda/blob/master/LICENSE)
