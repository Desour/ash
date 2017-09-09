# Ash

![screenshot](https://raw.githubusercontent.com/DS-Minetest/ash/master/screenshot.png)  
This mod adds ash when fire burns something.  

### API:  
Every flammable node without `on_burn` will be overridden to make ash on burn.  
If you want your node to make more ash, call in its `on_burn` `ash.burn_node(pos, param2)` a higher `param2`.

If you have a node that should be transformed to another node when ash is lying on it, do `ash.nodes_with_ash["your:node"] = "convert:to"` and `ash.nodes_with_ash[#ash.nodes_with_ash] = "your:node"`.  
You can also call `ash.ash_onto_node(pos)` if you want your node to be transformed directly. Note: `pos` is the position of the ash.  

### Licenses:  
Look into `license.txt`.  
[![image_CC0](https://licensebuttons.net/l/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)[![image_WTFPL](http://www.wtfpl.net/wp-content/uploads/2012/12/wtfpl-badge-1.png)](http://www.wtfpl.net/)[![image_CC_by_sa](https://licensebuttons.net/l/by-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-sa/4.0/)  