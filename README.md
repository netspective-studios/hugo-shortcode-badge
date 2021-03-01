# Hugo shortcode to render Badgen

The `badgen` Hugo shortcode renders [Badgen](https://shields.io/) supported badges from in markdown text. 
## Usage

Include this in your Hugo `config.yaml`:

```
module:
  imports:
    - path: github.com/netspective-studios/hugo-shortcode-badge
      mounts:
        - source: shortcodes
          target: layouts/shortcodes

```
If you are using `config.toml` in Hugo

```
[[module.imports]]
path                              = "github.com/netspective-studios/hugo-shortcode-badge"

[[module.imports.mounts]]
source                            = "shortcodes"
target                            = "layouts/shortcodes"

```
## Sample
```html
{{< badge renderHost="https://badgen.infra.medigy.com" subject="test" status="pending" color="red" scale="1.5" icon="github" >}}
```
