# crystal-web-demo

This is a demo of the [crystal-web](https://github.com/lbguilherme/crystal-web) package.

## Usage

Build with:

```sh
shards install
lib/web/scripts/build.sh src/demo.cr
```

If you want to optimize for release mode use:

```sh
shards install
lib/web/scripts/build.sh src/demo.cr --release
```

Create an index.html file with:

```html
<script src="demo.js"></script>
<script>runCrystalApp("demo.wasm")</script>
```

And start any web server to serve those files:

```sh
python3 -mhttp.server
```
