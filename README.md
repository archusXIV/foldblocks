# foldblocks
## A [lite-xl](https://github.com/lite-xl) plugin for folding/unfolding blocks of code

## About foldblocks
I use lite-xl since 2021 now and I love it, it's fast, elegant and customisable by using themes and plugins but I always missed a folding mechanism when I edit a file, specially when it's a big file. So I finally decide to create **foldblocks**. We can determine to use indicators in the gutter or not and the minimum number of lines in the block to enable folding/unfolding on the cursor position or selected line.
- [video](https://www.youtube.com/watch?v=3Fxj0s5Q6IY) (french spoken).
## Unfolded blocks
![screenshot without indicators](https://github.com/archusXIV/foldblocks/raw/main/screenshots/indicators_unfold.png)

## Folded blocks
![screenshot with indicators](https://github.com/archusXIV/foldblocks/raw/main/screenshots/indicators_fold.png)

## Configuration
Put this in your init.lua file to disable indicators.

```lua
config.plugins.foldblocks.indicators = false
```

Customizing the indicators symbols
```lua
config.plugins.foldblocks.indicator_open = "+"
config.plugins.foldblocks.indicator_closed = "-"
-- or
config.plugins.foldblocks.indicator_symbols = "+-"
```
Determine the minimum of lines to enable the folding mechanism (default is 2).

```lua
config.plugins.foldblocks.min_lines = 1
```

We can combine settings like this too.
```lua
config.plugins.foldblocks = {
    ["indicators"] = true,
    ["min_lines"] = 1,
    ["indicator_symbols"] = "+-"
}
```
To disable foldblocks (don't forget to comment out the other configurations).
```lua
config.plugins.foldblocks = false
-- config.plugins.foldblocks = {
--     ["indicators"] = true,
--     ["min_lines"] = 1,
--     ["indicator_symbols"] = "+-"
-- }
```
## How to use foldblocks

Once the plugin is configured, you can fold and unfold blocks of code using the following keybindings:

- `Ctrl+Alt+F` to fold the current block.
- `Ctrl+Alt+U` to unfold the current block.
- `Ctrl+Alt+A` to fold all blocks.
- `Ctrl+Alt+G` to unfold all blocks.
- `Ctrl+Alt+S` to fold the selected block.

You can also fold and unfold blocks by clicking on the indicators in the gutter if you have enabled them in the configuration. Note that the cursor must be on the first line of the block for the folding/unfolding actions to take effect.

Please report any [issues](https://github.com/archusXIV/foldblocks/issues) or feature requests on the [pull requests](https://github.com/archusXIV/foldblocks/pulls) pages.