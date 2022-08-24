# deps-infer

Infer `tools.deps` coordinates from a lib name, a partial set of coordinates, or both.

```
$ bbin install io.github.rads/deps-infer
{:lib io.github.rads/deps-infer,
 :coords
 {:git/url "https://github.com/rads/deps-infer",
  :git/tag "v0.0.1",
  :git/sha "cf7a85377fd05070135c0c5dcf606793de5d0560"}}
Cloning: https://github.com/rads/deps-infer
Checking out: https://github.com/rads/deps-infer at cf7a85377fd05070135c0c5dcf606793de5d0560

$ deps-infer --lib io.github.rads/deps-infer
#:io.github.rads{deps-infer #:git{:url "https://github.com/rads/deps-infer", :tag "v0.0.1", :sha "cf7a85377fd05070135c0c5dcf606793de5d0560"}}

$ deps-infer --lib io.github.rads/deps-infer --latest-sha
#:io.github.rads{deps-infer #:git{:url "https://github.com/rads/deps-infer", :sha "cf7a85377fd05070135c0c5dcf606793de5d0560"}}
```
