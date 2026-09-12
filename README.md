# foldblocks
## [lite-xl](https://github.com/lite-xl) plugin for folding/unfolding blocks of code

## About foldblocks
I use lite-xl since 2021 now and I love it, it's fast, elegant and customisable by using themes and plugins but I always missed a folding mechanism when I edit a file, specially when it's a big file. So I finally decide to create **foldblock**, we can determine to use indicators in the gutter or not and the minimum number of lines in the block to enable folding/unfolding on the particular line.

## Configuration
Put this in your init.lua file to enable indicators.

```
config.plugins.blockfold.indicators = true
```
Determine the minimum of lines to enable the folding mechanism (default is 2).

```
config.plugins.blockfold.min_lines = 1
```
