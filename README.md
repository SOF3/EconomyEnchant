# General

EconomyEnchant Shop For Pocketmine 4.0.0, With Many features

## Commands

Commands | Default
--- | ---
`/eshop` | True

## Feature
- Support Multiple Economys
- Support Multiple CustomEnchant
- Support EnchantTable Direct
- Auto Check Enchant Available in Hand
- Blacklist System
- Customable Message
- Customable Form

## Supported Custom Enchant Plugin
* [PiggyCustomEnchants](https://poggit.pmmp.io/p/PiggyCustomEnchants) by DaPigGuy
* [VanillaEC](https://poggit.pmmp.io/p/VanillaEC/) By David-pm-pl

## Supported Economy Providers

* [EconomyAPI](https://poggit.pmmp.io/p/EconomyAPI) by onebone/poggit-orphanage
* [BedrockEconomy](https://poggit.pmmp.io/p/BedrockEconomy) by cooldogedev
* [Capital](https://poggit.pmmp.io/p/Capital/) By SOF3

# Config

``` YAML

---
# Please don't edit this, only for internal use
config-version: 1

# Your Economy plugin name
# Available: BedrockEconomy, EconomyAPI, Capital, XP, Auto
# If you select auto but there is no Economy Plugin it will automatically use XP
economy: "Auto"

# Selector for Capital Economys
selector: []

# Label for Capital Economys
# use tag {name} For name Player, {price} For price Enchantment, {enchant} for Enchant Name
label-capital: "{name} has buyed {enchant} with price {price}"

# Can EnchantTable Redirect to EconomyEnchant
enchant-table: true

# Add Anvil Sound to Player if Enchant is Successful
sound: true

# Form
form:
 # Buy Menu
 buy-shop:
  # Title for BuyShop
  title: "EnchantShop"
  # Content for BuyShop
  content: "Select Enchantment:"
  # Button Style
  # Tag: {price} Price Enchantment, {enchant} Name Of Enchantment
  button:
   # Only can 0-1
   0: "{enchant}"
   1: "{price}"
 # Submit Menu
 submit:
  # Title for BuyShop
  title: "EnchantShop"
  # Content
  # Tag: {price} Price of Enchantment
  content: "§aYou will pay {price} Per Level"
  # Max Content
  max-content: "§aYour item has reached the level limit!"
  # Slider Content
  slider: "Level"

# Message
message:
 # Cannot Enchant On This Item
 err-item: "§cYou cannot add Enchantment to This Item!"
 # Exit Message
 exit: "§aThank you for visiting!"
 # Successfully Buy Enchant
 # Tag: {enchant} Name Enchantment, {item} Name Item, {price} Price Enchantment
 success: "§aSuccessfully Enchant {enchant} to {item}, with Price {price}"
 # Error Max Enchant
 max: "§cEnchant failed!, Your item is reached Max Level"
 # Error Money not Enough
 # Tag: {need} Needed Money
 enough: "§cYour money is not enough need {need}"

# Mode
# If false Enchantment those that are not set will not be in the shop
# If true Enchantment Auto added and price will be to Default ( Not Setted )
mode: true

# Enchantment
enchantment:
 # Name Enchantment
 sharpness:
  # Price
  price: 1000
 # Default, If the enchantment is not set above
 # it will be redirected here
 default:
  # Price
  price: 10000
  
# Blacklist Enchantment from Shop
# if you want blacklist just add
# example: ["sharpness", "silk_touch"] or ["sharpness"]
blacklist: []

# Blacklist Enchantment from Item
# if you want blacklist just add
# example: 
# blacklist:
#  sharpness: ["diamond_sword"]
# If you want add meta just item_name:meta
blacklist-item: []
...
```

# Additional Notes

- If you find bugs or want to give suggestions, please visit [here](https://github.com/MulqiGaming64/EconomyEnchant/issues)
