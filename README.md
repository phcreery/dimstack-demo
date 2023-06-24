## Demo site for dimstack

### Build

```
pdm build
cp '.\\dist\\*.whl' '.\\notebooks\\pypi\\'
cd notebooks
jupyter lite build --contents .
jupyter lite serve
```
