## Demo site for dimstack

## Usage

dimstack can be used in a standard python script, or as a REPL, allowing use in JupyterLab.

Demo usage in a JupyterLite Lab

- https://phcreery.github.io/dimstack-demo/lab/index.html

Demo usage in a JuptyerLite REPL:

- https://phcreery.github.io/dimstack-demo/repl/index.html?kernel=python&toolbar=1&code=%pip%20install%20-q%20ds%0Aimport%20dimstack%20as%20ds

Embed in your site:

```html
<iframe
  src="https://phcreery.github.io/dimstack-demo/repl/index.html?kernel=python&toolbar=1&code=%pip%20install%20-q%20ds%0Aimport%20dimstack%20as%20ds"
  width="100%"
  height="100%"
></iframe>
```

### Build

```
pdm build
cp '.\\dist\\*.whl' '.\\notebooks\\pypi\\'
cd notebooks
jupyter lite build --contents .
jupyter lite serve
```
