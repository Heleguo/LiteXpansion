# LiteXpansion 工业

LiteXpansion 是一个 Slimefun4 的附属插件，继承了来自 SlimeXpansion 的所有物品与部分功能。开发者正努力让此附属能提供类似工业2(IC2)模组的体验。

## :floppy_disk: 下载

<p align="center">
  <a href="https://builds.guizhanss.com/SlimefunGuguProject/LiteXpansion/master">
    <img src="https://builds.guizhanss.com/f/SlimefunGuguProject/LiteXpansion/master/badge.svg" alt="Build status"/>
  </a>
</p>

## :gear: 配置

### config.yml

你可以修改两个配置项：

- `auto-update` - 启用后会开启自动更新 (默认: `true`)
- `nerf-other-addons` - 启用后会削弱其他附属中的发电机（下方已列出），禁用则会使本附属插件中机器电力消耗翻倍 (默认: `true`)
  - 粘液科技 - 充能太阳能板
  - 无尽科技 - 所有发电机
  - 战争工艺 - 元素发电机
  - 星际 - 聚变反应堆
  - 至尊研究院2.0 - 所有发电机

### uumatter.yml

如需添加、删除或修改配方，你需要修改 `/plugins/LiteXpansion/uumatter.yml` 文件。

在 `recipes` 下，你可以指定输出的物品，这可以是 [原版物品ID](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Material.html) 或是 Slimefun 物品ID (支持附属插件)。如果你想让输出的物品数量多于1，你可以在物品ID后面加上一个英文的冒号(`:`)与数量。在接下来的合成表中，`x`代表UU物质，空格为无物品。

以下是一个合成20个煤炭的例子:

```yaml
recipes:
  # 输出的物品, 使用冒号 (:) 来指定数量
  # 可使用原版物品ID (https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Material.html) 或 Slimefun 物品ID
  'COAL:20':
    # 合成表, x = UU物质, 空格 = 无物品
    - '  x'
    - 'x  '
    - '  x'
```

### :computer: Discord

如果你想找到一个 Slimefun 物品的ID，你可以通过下方的图片链接加入我们的官方 Slimefun Discord 服务器，并在`#bot-spam`频道中发送`!item <name/ID>`即可获取。

你也可以在`#litexpansion`频道中讨论任何有关 LiteXpansion 的内容。

<<<<<<< HEAD
[加入Slimefun 官方Discord服务器](https://discord.gg/slimefun)
=======
<p align="center">
  <a href="https://discord.gg/slimefun">
    <img src="https://discordapp.com/api/guilds/565557184348422174/widget.png?style=banner3" alt="Discord Invite"/>
  </a>
</p>

### 📥 Compilation
To be able to compile this source,
you need to get yourself [BuildTools](https://www.spigotmc.org/wiki/buildtools/) from SpigotMC and
create 1.20.4 Minecraft mappings - NMS which are being used in [NMS_1.20.4_Enchants](NMS_1.20.4_Enchants)
<br><b>Help-line: ``java -jar .\BuildTools.jar --remapped --rev 1.20.4``
>>>>>>> 10930c6c0e1316dbba73f46b90825adf275209f4
