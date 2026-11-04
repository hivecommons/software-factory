# software-factory

The Spek → Hive "software factory" motion graphic: a single self-contained HTML file
(no external dependencies) showing how a specification becomes a merged, verified pull
request. It is served by GitHub Pages at <https://hivecommons.dev/software-factory/> and
embedded as the hero section of [hivecommons.dev](https://hivecommons.dev).

## URL parameters

| Param | Values | Notes |
| --- | --- | --- |
| `flow` | `spek` \| `full` | `spek` = Spek → Hive; `full` = Spotlight → Nous → Spek → Hive |
| `speed` | number | relative to the default tempo (`1` = default) |
| `mode` | `present` | hides the page chrome (used by the homepage embed) |
| `theme` | `light` \| `dark` | omit to follow `prefers-color-scheme` |
| `loop` | `short` \| ms | loop length |
| `motion` | `reduce` | reduced-motion variant |
| `t` | ms | freeze the animation at a point in time |

Example: <https://hivecommons.dev/software-factory/?flow=spek&speed=1&mode=present>

## Re-syncing

`index.html` is copied verbatim from the authoring build; do not edit it here.

```sh
cp ~/Downloads/software-factory.html index.html && git commit -s -am "sync" && git push
```

## License

[Apache-2.0](LICENSE)
