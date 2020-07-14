# minecraft-lists

A list of every item and block in the game.

## Methodology

*Note: Requires some technical knowledge to understand*

To ensure the accuracy of the item list, I decompiled Minecraft (though I don't use/can't find a de-obfuscated version) and searched for a few test items to find the relevant classes (note to anoyone DIYing this: `bvs.class` contains block IDs, and `bkk.class` contains non-block item IDs). Interestingly, any items which are placeable as blocks have their IDs listed _only_ in the list of block IDs. To get the final list, one has to reference back and forth between the classes. I did so using a node.js program, and grep for debugging.

For blocks, it's much simpler. All I had to do was extract all of the relevant strings. no cross-referencing or bug hunting necessary.

## Contributing

If you think an additional list should be added, such as for older versions or things like entities or particles, make a comment or pull request and I'll check it out. Hopefully these lists comes in handy for some people!
