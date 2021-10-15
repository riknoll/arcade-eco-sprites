# arcade-eco-sprites

A collection of sprites with environmental themes.

To build these sprites:

```
pxt target arcade
pxt install
pxt buildsprites .
```

To add new sprites, create a `.png` and add it to the assets folder. Then create a `.json` file with the same name and place it next to the image. The JSON should be of this format:

```json
{
    "width": 40,
    "height": 40,
    "frames": [
        "stumps1",
        "stumps2",
        "clouds1",
        "clouds2",
        "burntTrees",
        "frozenTree",
        "mountain",
        "meltedIceberg",
        "tree1",
        "tree2",
        "volcano",
        "iceberg"
    ],
    "animations": [],
    "tags": "misc"
}
```

Make sure the frames array has an entry for every sprite inside the `.png`. Additionally, all sprites in the `.png` should be the same size. `width` and `height` refer to the individual sprites and not the entire image.

#### Metadata (used for search, rendering)

* for PXT/arcade