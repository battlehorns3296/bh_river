# A Battlehorns improved version of the syn_river plugin

## Requirements
- [VORP_Core](https://github.com/VORPCORE/vorp-core-lua)
- [fred_metabolism](https://github.com/SirFreddie/fred_metabolism_free)
- [VORP Inventory](https://github.com/VORPCORE/vorp_inventory-lua)
- And all requirements from the above required Plugins

## How to install
* Download the lastest release version of bh_river
* Copy and paste ```bh_river``` folder inside ```resources``` folder or any folder with ```[]``` name in it
* Copy ```img``` folder content into ```vorp_inventory/html/img/``` folder
* Import the SQL file inside ```sql``` folder into your database
If you got erros on the SQL import, please check if you dont have already a duplicated record on your ```items``` MySQL table
* Add all the items to for you be able to consume apart from the ```empty``` one(that should not be used as drinkable) into your metabolism plugin config file
* Edit those items on Metabolism plugin to your needs
* Finally add ```ensure bh_river``` to your ```resource.cfg``` or ```server.cfg``` file depending where you have your resources to be loaded.

* To edit the languages go to ```languages``` folder
* To add new languages just duplicate the files already there and edit the name of the new one relative to the config file.

## Example

from
```lua
Locales["en"] = {
  fill_Canteen_Button     = "Fill Canteen",       --Button Names
  fill_Bucket_Button      = "Fill Bucket",        -- ""
.....
```
into
```lua
Locales["xx"] = {
  fill_Canteen_Button     = "Fill Canteen in XX language",       --Button Names
  fill_Bucket_Button      = "Fill Bucket in XX language",        -- ""
.....
```
config.lua
```lua
Config = {}

-- Active language/locale
Config.defaultlang = "xx"
```

## Features
* Small drink amount from the river
* Fill Canteen from river
* Drink from Canteen reduce 20% of the Canteen content
* You dont need to drink the full content of the Canteen to refill it from the river
* You can quick refresh yourself from the river
## TODO
* You can fill your bucket of water from the river to use it to water your crops
* Add items to the Character hands while on the animation
* Add more Config options into the ```config.lua``` file
* And more...

## Credits
- to [blue](https://github.com/kamelzarandah) for the initial work on the syn_river plugin

## Our Community
[WEBSITE](https://www.battlehorns.net)
[DISCORD](https://discord.gg/59pmYGHEtD)
