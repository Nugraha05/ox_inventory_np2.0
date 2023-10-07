<div align='center'><img src='https://cdn.discordapp.com/attachments/687859445958443048/1160060962615853117/image.png?ex=653349f6&is=6520d4f6&hm=b3476e301e4b18d7bc81e58fe502c947f8a0734ca3c35ba99f4449742da92c3b&'/></div>

<div align='center'><h3><a href='https://overextended.github.io/docs/ox_inventory/'>Read the documentation for setup, installation, and integration</a></h3></div>

# Preview
<div align='center'><img src='https://cdn.discordapp.com/attachments/687859445958443048/1160060808705884280/image.png?ex=653349d1&is=6520d4d1&hm=e8dad6f96fde2dbf264560b91ffb500c5b8b73db10c898169a227c642249aa98&'/></div>
<div align='center'><img src='https://cdn.discordapp.com/attachments/687859445958443048/1160060652942020678/image.png?ex=653349ac&is=6520d4ac&hm=dfff8915fd1a87bdb5d3a891e9abde65de3eb2548955c5cf22befd645bd4586a&'/></div>
<div align='center'><img src='https://cdn.discordapp.com/attachments/687859445958443048/1160061527009796096/image.png?ex=65334a7c&is=6520d57c&hm=79011e9dc93163c6a2a0b3f1a6a353fa9917b7d671b6d9154c22df306609614a&'/></div>
<div align='center'><img src='https://cdn.discordapp.com/attachments/687859445958443048/1160061527009796096/image.png?ex=65334a7c&is=6520d57c&hm=79011e9dc93163c6a2a0b3f1a6a353fa9917b7d671b6d9154c22df306609614a&'/></div>
<div align='center'><img src='https://cdn.discordapp.com/attachments/687859445958443048/1160057041520443422/image.png?ex=6533464f&is=6520d14f&hm=f70dd91246fa6078d6787805854f73b76d3626e19bc502a46f6a26e6c5f12e9f&'/></div>

# Framework

The inventory was designed with the intention to move towards a more generic / standalone structure so it can be integrated into any framework without too much hassle. I will be writing a guide for manually setting up support _sometime soon™_. In the mean-time, it will work without any alterations if using the latest updates to **[ESX Legacy](https://github.com/esx-framework/esx-legacy)**.

Experimental support for [qb-core](https://github.com/qbcore-framework/qb-core) has been added, but requires a recent installation. Do not expect 100% compatibility or support.

# Config

Refer to the [documentation](https://overextended.github.io/docs/ox_inventory/) setting your config.
When set, you can add the following to your 'server.cfg'

```
exec @ox_inventory/config.cfg
ensure ox_inventory
```

# Logging

The included logging module utilises datadog to store logging data, which can be expanded for improved analytics and metrics. Register an account at [datadoghq](https://www.datadoghq.com/).
The _free plan_ is enough for most user's purposes and provides far more utility than the typical weird discord logs utilised in other resources.

Once you have registered, generate an API key and add `set datadog:key 'apikey'` to your server config.

# Features

### Shops

- Creates different shops for 24/7, Ammunation, Liquor Stores, Vending Machines, etc.
- Job restricted shops, such as a Police Armoury.
- Items can be restricted to specific job grades and licenses.
- Define the price for each item, and even allow different currency (black money, poker chips, etc).

### Items

- Generic item data shared between objects.
- Specific data stored per-slot, with metadata to hold custom information.
- Weapons, attachments, and durability.
- Flexible item use allows for progress bars, server callbacks, and cancellation with simple functions and exports.
- Support for items registered with ESX.

### Stashes

- Server-side security prevents arbitrary access to any stash.
- Support personal stashes, able to be opened with different identifiers.
- Job-restricted stashes as well as a police evidence locker.
- Server exports allow for registration of stashes from any resource (see [here](https://github.com/overextended/ox_inventory_examples/blob/main/server.lua)).
- Access small stashes via containers, such as paperbags, from using an item.
- Vehicle gloveboxes and trunks, for both owned and unowned.

### Temporary stashes

- Dumpsters, drops, and non-player vehicles.
- Loot tables allow users to find random items in dumpsters and unowned vehicles.

<br><div><h4 align='center'><a href='https://discord.gg/hmcmv3P7YW'>Discord Server</a></h4></div><br>

<table><tr><td><h3 align='center'>Legal Notices</h2></tr></td>
<tr><td>
Ox Inventory

Copyright © 2022 [Linden](https://github.com/thelindat), [Dunak](https://github.com/dunak-debug), [Luke](https://github.com/LukeWasTakenn)

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.
If not, see <https://www.gnu.org/licenses/>

</td></tr></table>
