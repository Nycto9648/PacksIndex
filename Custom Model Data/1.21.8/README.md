# Custom Model Data 1.21.8

After specifing item in your /give command, the part [minecraft:custom_model_data={floats:[1f]}] tells Minecraft which custom model to use from your resource pack. Lets look at each part.

`minecraft:custom_model_data` – signals the game to check for model overrides.

`{floats:[1f]}` – a list of floats; here 1f matches the float value in your JSON override:

"predicate": {
  "minecraft:custom_model_data": { "floats": [1.0] }
}


Minecraft replaces the default model with the matching override.

Using floats allows for more precision and multiple model options than the old integer-only system.
