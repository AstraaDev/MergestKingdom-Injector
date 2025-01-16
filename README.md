<p align="center">
  <img src="https://imgs.crazygames.com/mergest-kingdom_16x9/20241211151323/mergest-kingdom_16x9-cover?auto=format%2Ccompress" width="600">
</p>

<h1 align="center">[Discord] - Mergest Kingdom Injector</h1>

<p align="left">
  Mergest Kingdom Injector lets you set up various methods for modifying content in the Mergest Kingdom discord game. Perform these steps preferably from a Google Chrome browser. There is currently no guarantee that these methods will work on other browsers.
  These methods go against the rules of the game's developers, and waves of bans have already occurred. I am in no way responsible for your actions. Please use this tool with full knowledge of the risks involved.
</p>


## Disclaimer

|Mergest Kingdom Injector was made for Educational purposes   |
|-------------------------------------------------|
This project was created only for good purposes and personal use.
By using this Tool, you agree that you hold responsibility and accountability of any consequences caused by your actions.

## Features

- [x] - [giveInventoryItem](https://github.com/AstraaDev/MergestKingdom-Injector) - Obtain any object in unlimited quantities.

## [METHOD] : giveInventoryItem
<details>
<summary>What you can get with this method ?</summary>

### Consumable

| Parameter                         | Description                      |
| :-------------------------------- | :------------------------------- |
| `exp`                             | Experience                       |
| `energy`                          | Energy for activities            |
| `rubies`                          | Purple rubies                    |
| `soft`                            | Golds                            |
| `wands `                          | Keys                             |

</details>
<details>
<summary>Click to expand the information</summary>

- Launch of Mergest Kingdom on discord *(and never close it again until the end)*
- Open the browser console (by pressing `CTRL`+`SHIFT`+`I` on Windows/Linux or `Cmd`+`Opt`+`I` on MacOS)
- In the **SOURCE** tab, find the file named game.js located at `top/12766.discordsays.com/12766.discordsays.com/.proxy/static/game.js` *(see image below)*
<img src="img/readme_screenshot/MK_1.png" width="400">

- In `game.js` file,
- Search the file (by pressing `CTRL+`F`)
- Write the following command and press `ENTER` :
```js
RewardTypes[this.type].handler.call(this, this.value, this.options)
```
- There will normally be `1` results. Navigate to this one and set a breakpoint by clicking on the left of the line in the grey area *(see image below)*
<img src="img/readme_screenshot/MK_2.png" width="500">

- Return to the game and collect an object *(the game should stop again)*
- In the **SOURCE** tab, find the type and value arguments at `Local/this` *(see image below)*
<img src="img/readme_screenshot/MK_3.png" width="300">

- Replace `type` with the item you want *(the list is available above)* and `value` with the quantity you want *(see image below)*
<img src="img/readme_screenshot/MK_4.png" width="300">

- You can now go back to the `game.js` file in the **SOURCE** tab, then remove the breakpoint *(by clicking on it again)* and click on the `Resume script execution` button again
- Your item should be added.
</details>

## Additional Informations
Discord :
- Any question ? Any malfunction ? Contact me on [here](discord.gg/PKR7nM9j9U).
