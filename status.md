# where are we now

fontmake does not support two axes + bracket layers. One axis + bracket layer, yes; two axes, yes. (Maybe a solution to release `Open Sans VF` and `Open Sans Condensed VF`?) Because of the fontmake issues, I am doing fixes from these diffs as hotfixes in the TTFs and then fixing in source instead of building from source again.

### good

1. `OpenSans-Roman-VF.ttf` and `OpenSans-Italic-VF.ttf` are hinted fonts with the variable substitutions working correctly
2. Roman kerns match 100%
3. Hinted instances look like they match 100% according to diffenator

### to-dos

1. `a` interpolates poorly
2. add kerning to italic TTF
3. mkmk positioning is built automatically by Glyphs so no tuning is possible there: will see if this is worth tuning

### needs tested

1. OpenType substitutions
2. vert metrics
3. italic kerning

### notes on diffs

1. Mac names are gone now
1. all combining accents now have zeroed sidebearings to match best practices and so they diff
1. `uni0478` / `Ѹ` renders incorrectly in ExtraBold & -Condensed: metrics and shaping is correct in source
2. `.numr` or `superior` figures appear to be rendering incorrectly: they match in source
3. `g894` is an unencoded accent and shows incorrect metrics but sources match
4. diffs for marks (esp. `mkmk`) are good: they were initially incorrect