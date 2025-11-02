# 🛠️ Custom Model Data 1.21.8-1.21.10 🛠️

After specifying the item in your /give command, the part `[minecraft:custom_model_data={floats:[1f]}]` tells Minecraft which custom model to use from your resource pack.

`minecraft:custom_model_data=` – signals the game to look for any model overrides for this item.

`{floats:[1f]}` – a list of float values; here, 1f corresponds to the float specified in your JSON override.


#### Full Correct Command
`/give @s minecraft:paper[minecraft:custom_model_data={floats:[1.0f]}]`
