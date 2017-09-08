# Ash

![screenshot](https://raw.githubusercontent.com/DS-Minetest/ash/master/screenshot.png)  
This mod adds ash when fire burns something.  


Every flammable node without `on_burn` will be overridden to make ash on burn.  
If you want your node to make more ash, call in its `on_burn` `ash.burn_node(pos, param2)` a higher `param2`.

If you have a node that should be transformed to another node when ash is lying on it, do `ash.nodes_with_ash["your:node"] = "convert:to"` and `ash.nodes_with_ash[#ash.nodes_with_ash] = "your:node"`.  
You can also call `ash.ash_onto_node(pos)` if you want your node to be transformed directly. Note: `pos` is the position of the ash.  