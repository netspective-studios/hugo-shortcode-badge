# Hugo shortcode to render Badge

The `badge` Hugo shortcode renders [Badgen](https://badgen.net/) supported badges from in markdown text. 
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
{{< badge renderHost="https://badgen.infra.medigy.com" subject="Community%20of%20Practice" status="Join" color="green" scale="1.5" icon="github" >}}
```
## Sample HTTPS Service (upvote-count)
```html
{{< badge renderHost="https://badgen.infra.medigy.com" httpsService="true" serviceRequestFor="upvote-count" offeringIdentifier="9465" >}}
```