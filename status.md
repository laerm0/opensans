# where are we now

fontmake does not support two axes + bracket layers. One axis + bracket layer, sure (is a solution to release `Open Sans VF` and `Open Sans Condensed VF`?

### good

4. `OpenSans-Roman-VF.ttf` and `OpenSans-Italic-VF.ttf` are hinted fonts with the variable substitutions working correctly
2. 
3. 

### bad

1. `a` interpolates poorly
2. add kerning to italic TTF
3. mkmk positioning is built automatically by Glyphs so no tuning is possible there

### needs tested

1. OpenType
3. italic kerning

### notes on diffs
1. `uni0478` / `Ѹ` renders incorrectly in ExtraBold & -Condensed: metrics and shaping is correct in source
2. 