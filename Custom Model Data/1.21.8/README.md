# Custom Model Data 1.21.8

After specifying the item in your /give command, the part [minecraft:custom_model_data={floats:[1f]}] tells Minecraft which custom model to use from your resource pack.

`minecraft:custom_model_data` – signals the game to check for model overrides.

`{floats:[1f]}` – a list of floats; here 1f matches the float value in your JSON override.

#### Full Correct Command
`/give @s minecraft:paper[minecraft:custom_model_data={floats:[1.0f]}]`
