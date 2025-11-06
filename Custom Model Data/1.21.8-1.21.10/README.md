# 📘 Custom Model Data – Data Component Format

## `minecraft:custom_model_data`
- **Type:** `[NBT Compound / JSON Object]`  
- **Purpose:** Container of values used by item model definitions for **model selection** and **coloring**.

---

## `floats`
- **Type:** `[NBT List / JSON Array]` of `[Float]`  
- **Used for:** The **range_dispatch** model type (selects a model based on a range of floats).  
- **Behavior:** If no matching value is found, the **fallback model** is used.

---

## `flags`
- **Type:** `[Byte Array]` (list of booleans)  
- **Used for:** The **condition** model type (model selection based on boolean flags).  
- **Behavior:** Missing values use the **is_false** model.

---

## `strings`
- **Type:** `[NBT List / JSON Array]` of `[String]`  
- **Used for:** The **select** model type (chooses models based on string values).  
- **Behavior:** If none match, the **fallback model** is used.

---

## `colors`
- **Type:** `[NBT List / JSON Array]` or `[Int Array]`  
- **Purpose:** Provides RGB values for tints applied by the model type’s coloring logic.  
- **Details:**  
  - Each entry may be a list of floats or an integer.  
  - Lists of floats are **automatically converted to integers** internally.  
  - Missing values use the default color from the item model definition.

---

## 🔍 Why This Matters
This format allows resource pack makers to define detailed custom models with advanced selection logic, including:
- Choosing models based on numeric ranges (`floats`)  
- Using boolean flags (`flags`)  
- Matching text strings (`strings`)  
- Applying custom color tints (`colors`)

It provides much more flexibility than the older integer-only model override system.
