# RLCraft 入坑指南 调整建议 添加内容 开服相关

# 简介 

![img](https://i0.hdslb.com/bfs/article/0117cbba35e51b0bce5f8c2f6a838e8a087e8ee7.png@progressive.webp)

　　RLCraft是一个追求写实和养老生活的Minecraft整合包，专注于生存、冒险、RPG和沉浸感。这个整合包加入了许多符合冒险和生活风格的模组，并且通过针对性的调整使他们围绕同一个沉浸生存的主题。

　　RLCraft修改了许多Minecraft原版的机制，适合在原版的基础上更想体验冒险内容的玩家。对于刚刚上手Minecraft的玩家内容可能有些繁杂，但是如果有一定RPG游戏经验的玩家直接上手RLCraft也是不难的。

　　作为Minecraft的一个整合包，在游玩RLCraft时除了单纯的冒险和战斗，在多个维度里对世界进行改造和创造也是重要的内容，这些内容能逐渐在冒险中发挥显著的作用。

入坑指南

![img](https://i0.hdslb.com/bfs/article/0117cbba35e51b0bce5f8c2f6a838e8a087e8ee7.png@progressive.webp)

　　RLCraft整合包官方发布于CurseForge，在各个启动器的整合包下载功能均能下载，MultiMC等现不支持CurseForge整合包的启动器可以在CurseForge网站直接下载开服包（Server Pack）作为客户端游玩（内容与客户端整合包稍有区别，可以互通）。

**CurseForge**：https://www.curseforge.com/minecraft/modpacks/rlcraft

**MCBBS**：https://www.mcbbs.net/thread-927630-1-1.html

**MC模组百科**：https://www.mcmod.cn/modpack/16.html

**RLCraft官方百科**：https://rlcraft.fandom.com/wiki/RLCraft_Wiki



　　推荐查看本文调整建议和添加内容两节，调整建议是当前版本建议做的重要调整，添加内容包含部分强烈推荐实际游玩时添加的模组和设置。
　　RLCraft的汉化推荐使用自动汉化更新（I18nUpdateMod）模组，或手动下载汉化资源包，任务书文本内容意义极少，可以选择不汉化或者在专栏搜索RLCraft任务书汉化。

**自动汉化更新**：https://www.mcmod.cn/class/1188.html

**汉化资源包**：https://github.com/CFPAOrg/Minecraft-Mod-Language-Package/releases

　　RLCraft基于MC1.12.2，需要使用jre8启动，作者推荐分配3～4GB内存启动，推荐JVM参数：

```javascript
-Xmx4G -XX:+UseConcMarkSweepGC -XX:+CMSIncrementalMode -XX:-UseAdaptiveSizePolicy -Xmn128M
```

　　实际游玩可以提高内存分配，6～8GB足以流畅运行当前版本的RLCraft，推荐JVM参数：

```javascript
-server -Xss512K -XX:MaxGCPauseMillis=25 -XX:+UnlockExperimentalVMOptions -XX:+UseGCOverheadLimit -XX:+ParallelRefProcEnabled -XX:-OmitStackTraceInFastThrow -XX:+UseCompressedOops -XX:+PerfDisableSharedMem -XX:+ExitOnOutOfMemoryError -XX:+AlwaysPreTouch -XX:+TrustFinalNonStaticFields -XX:+UseFastUnorderedTimeStamps -XX:+DisableExplicitGC -XX:-UseParallelGC -XX:+UseG1GC -XX:TargetSurvivorRatio=90 -XX:G1NewSizePercent=50 -XX:G1MaxNewSizePercent=80 -XX:G1MixedGCLiveThresholdPercent=35
```



Minecraft基础游玩问题可以参考官方百科

https://minecraft.fandom.com/zh/wiki/Minecraft_Wiki

RLCraft基本游玩问题可以参考MCBBS搬运贴《**快速游玩指南**》和网络资料

![img](https://i0.hdslb.com/bfs/article/c8f606f35dc76cf1eba08fbdaec7c1a70d409d9b.png@1256w_708h_!web-article-pic.webp)入坑指南

调整建议

![img](https://i0.hdslb.com/bfs/article/0117cbba35e51b0bce5f8c2f6a838e8a087e8ee7.png@progressive.webp)

　　**设置包**：

　　首先强烈推荐安装作者提供的硬核设置包（HARDCORE Config Pack，注意不是HARDCORE Server Setup），这个设置包在当前版本上进一步调整了游戏平衡，修复了一个关键的结构生成错误和调整众多内容更加符合整合包主题。

　　硬核模式玩家可以考虑上面提到的服务器硬核模式包（HARDCORE Server Setup），它的主要内容是使得玩家死亡时重置RPG内容的进度，用于服务器不封禁玩家的硬核模式，也可以在单人用作保留存档的硬核模式。

　　注意两个设置包同时安装时，需要先安装服务器硬核模式包，再安装硬核设置包。

**硬核设置包**：https://www.curseforge.com/minecraft/modpacks/rlcraft/files/3814632

**服务器硬核模式包**：https://www.curseforge.com/minecraft/modpacks/rlcraft/files/3814642



　　**性能问题**：RLCraft包含几个性能消耗较大的装饰性模组，可以几乎不影响游玩而安全地移除或者根据需求调整设置：

- 更好的树叶（Better Foliage）：更茂盛的树叶。性能消耗很大，与部分资源包和光影不兼容
- 梦幻方块效果（Fancy Block Particles）：更好的方块放置/破坏特效。性能消耗较大，效果高度可配置
- 更多弯曲（Mo' Bends）：给玩家和生物增加关节动作。性能消耗较大，是RLCraft冒险体验的特色之一，不建议移除
- 物理掉落完整版（ItemPhysic Full）：更真实的物品掉落和掉落物交互方式。性能消耗较大，对于RLCraft游玩有交互体验上的影响，不建议移除
- 区块加载动画（Chunk Animator）：使得区块加载时不那么突兀。性能消耗较小，有多种样式可以选择

除物品物理掉落完整版（ItemPhysic Full）外，移除这些模组都不会影响多人连接。



　　**自助内容更新**：

　　RLCraft作者在当前版本有意避免了使用几个模组的最新版本，同时RLCraft也有一段时间没有更新了，有些模组更新了重要内容。其中最重要的是冰与火之歌（Ice and Fire）模组增加了一级龙钢科技，在RLCraft是30级攻击/防御定位的内容。

- **冰与火之歌（Ice and Fire）**：更新冰与火之歌至1.9.1，需要同时更新斯巴达之冰与火（Spartan and Fire）至0.08，并将ISeeDragons的配置文件中B:DragonLag设置为false。
- 实体渲染机制优化（Entity Culling）：直接更新至最新1.12.2版本即可
- ModTweaker：直接更新至最新版本即可
- RLTweaker：直接更新至最新版本即可



　　**推荐资源包和光影**：

　　Chroma Hills可以说是RLCraft官方推荐资源包，其风格很贴合RLCraft的生存沉浸感。Lycanites Redux是一个为恐怖生物（Lycanites Mobs）模组的生物提供MC风格贴图的资源包（恐怖生物自身的贴图在MC里比较突兀），强烈推荐使用。

　　对于Chroma Hills或者其他资源包没有覆盖材质的模组，可以使用Faithful风格模组资源包提供接近原版风格的高清材质。对于喜欢原版风格材质包的玩家，也推荐Faithful原版资源包。需要注意Faithful原版资源包和Chroma Hills同时使用会导致玻璃等贴图错误，不建议同时加载。

　　同时，RLCraft自带的"LycanitesMobs32X.zip","Lum.1.12.2.zip","AnimEmis_InF_SW_Blue.zip","RLHats.zip"和汉化资源包"Minecraft-Mod-Language-Modpack.zip"也建议加载。



　　光影需要添加OptiFine或者其他光影模组使用，对于RLCraft的风格推荐Sildurs Shaders或SEUS，其他对于一般生存友好的光影还推荐UShader，Chocapic13' Shaders，AstraLex Shaders和Complementary Reimagined。

注意大多光影都会与动态环境（Dynamic Surroundings）、实体渲染机制优化（Entity Culling）和更好的树叶（Better Foliage）有一定冲突。动态环境的极光（Aurora）通常渲染效果不佳，可以考虑关闭；脚印渲染出现问题时可以尝试更换脚印类型或者材质。实体渲染机制优化可能导致光影穿墙渲染实体和光照，可以尝试禁止被命名的实体渲染优化，或者完全去除该模组。更好的树叶可能导致树叶材质错误或者树叶阴影渲染问题。



**资源包**

**Lycanites Redux**：https://www.curseforge.com/minecraft/texture-packs/lycanites-redux

Chroma Hills：https://www.chromahills.com/

Faithful：https://faithfulpack.net/downloads

Faithful风格模组资源包（新项目）：https://faithfulpack.net/modpacks

Faithful风格模组资源包（旧项目）：http://f32.me/



**光影**

Sildurs Shaders：https://sildurs-shaders.github.io/downloads/

SEUS：https://www.sonicether.com/seus/

UShader：https://www.curseforge.com/minecraft/customization/ushader

Chocapic13' Shaders：https://www.curseforge.com/minecraft/customization/chocapic13-shaders

AstraLex Shaders：https://www.curseforge.com/minecraft/customization/astralex-shader-bsl-edit

Complementary Reimagined：https://www.curseforge.com/minecraft/customization/complementary-reimagined

![img](https://i0.hdslb.com/bfs/article/53a7787b5ee7a9aa5727c9dc91805b84b8d0e51a.png@1256w_708h_!web-article-pic.webp)调整建议



# 添加内容

![img](https://i0.hdslb.com/bfs/article/0117cbba35e51b0bce5f8c2f6a838e8a087e8ee7.png@progressive.webp)

　　**开启/配置机制**：

- Scaling Health内置**高级动态难度**设置，作者的硬核设置包已经开启，不论是否使用硬核设置包都建议开启这个功能并且按需求手动设置
- Scaling Health可以开启自定义血量渲染和替换原版血条，得到比较**简洁的血条**：main{client{B:"Custom Heart Rendering"=true,B:"Replace Vanilla Heart Row With Custom"=true}}
- 急救（First Aid）提供多种部位血量显示模式，设置为HEARTS或者NUMBERS可以得到直观准确的部位血量显示：general{overlay{S:overlayMode}}
- 全局游戏规则（Global GameRules）可以修改**游戏规则**，其中RLCraft的**出生范围**gamerules{S:spawnRadius}默认为10000，可以根据需求缩小聚集玩家或者放大分散玩家
- Corpse Complex可以开启**死亡惩罚**系统，并且根据需求修改死亡惩罚效果
- 升级！重置（Level Up!Reloaded）的合成经验黑名单blacklist{S:CraftingOutputs}建议加入以下内容，限制一些过于简单的经验获取方式

```javascript
minecraft:wool
quark:quilted_wool
minecraft:dye
```

- 指路石（Waystones）建议关闭短距离免经验传送，避免连续短距离传送规避经验消耗：general{B:"Short Travel is Free"=false}
- 古式地图（Antique Atlas）可以设置**迷你地图**不需要手持古式地图，如果不添加其他地图模组建议开启：atlas_overlay.cfg中appearance{B:requiresHold=false}
- 动态环境（Dynamic Surroundings）在使用光影时推荐关闭极光（Aurora）；多人游玩推荐开启**聊天气泡**（Speech Bubbles）
- R键整理 （Inventory Tweaks）可以自定义排序和栏位规则，对于背包管理帮助很大
- 更好的任务（Better Questing）可以为新人开启任务提示，获得更好的任务指引：general{B:"Quest Notices"=true}

　　**常用模组**：

- 自动汉化更新（I18nUpdateMod）：自动更新汉化资源包
- 窗口化全屏（Fullscreen Windowed）：窗口全屏，现代游戏都应该有的体验
- 高清修复（OptiFine）：大量渲染优化和功能，也包含光影支持。但是同时也存在一些问题，区块加载动画（Chunk Animator）需要关闭区域渲染才能正常生效
- Nothirium：区块渲染优化，建议配合高清修复使用。会使得高清修复的动态光源和智能材质失效（智能材质Nothirium提供了更好的优化）
- 平滑字体（Smooth Font）：字体渲染优化，也提供更改字体的功能
- 简单村民交易（EasierVillagerTrading）：简化和村民的交易，RLCraft有和村民交易的需求
- ReAuth：账号掉线重连
- 按键精灵（Keyboard Wizard）：方便直观的按键设置，用于解决按键冲突和分配按键

这些模组都不会影响多人连接

　　**其他内容推荐**：

- Serene Tweaks：使得静谧四季（Serene Seasons）冬天下的雪换季后未加载区块的雪融化，对于环境的沉浸感十分重要。
- 真实昼夜循环（Accurate day/night-cycles）：调整游戏日的时间，天象，与静谧四季（Serene Seasons）的季节联动获得更真实的季节时间。
- 物品栏HUD+（Inventory HUD+）：调整游戏界面，包括背包预览，药水效果和武器护甲饰品显示。药水效果设置成迷你模式，最大10分钟时对葡萄酒适配很好。建议配合关闭动态环境（Dynamic Surroundings）的药水效果显示和移除斯巴达饰品栏HUD（Spartan HUD: Baubles）
- 游戏阶段（Game Stages）：根据“游戏阶段”控制物品、生物和机制的有效性。RLCraft有很多内容自带对游戏阶段的联动可以开启，也方便增加更多科技树限制。使用需要一定魔改基础
- 玩家救援（PlayerRevive）：战斗复活，解决多人冒险有人死亡掉队的问题，或者在极限模式多人多给一个挽回的方法
- 墓碑 (GraveStone)：死亡产生墓碑，保护掉落物来降低回收物品的难度。不推荐
- 魔法使（Mahou Tsukai）：给RLCraft增添一套风格相符的魔法系统。建议参考作者提供的1.19平衡配置修改数值平衡，用Reskillable和游戏阶段限制魔法使作为中期魔法科技。由于葡萄酒的存在，魔法使很多本身持续时间较短的药水效果价值被提高了，需要进行平衡。另外为了平衡和操作方便也建议在搬运（Carry On）模组中禁用搬运魔法使的方块。整体来说风格和强度都适合RLCraft
- 暮色森林（The Twilight Forest）：添加一个完善的冒险世界，除了本身较符合RLCraft以外，可以给上手RLCraft有困难的新人一个更刺激的前期路线。建议给暮色森林的道具设置门槛，并且提供套装效果。为了RLCraft内容的平衡建议关闭拆解台拆解功能，为了世界生成性能需要调整生成参数，这两点详细见MC模组百科
- 更好的建筑之杖（Better Builder's Wands）：生存友好的建筑辅助工具。RLCraft作者希望RLCraft成为一个可以养老的冒险整合包，那么建筑方面也需要补充一些辅助功能
- 凿子（Chisel）：另一个建筑模组，提供多种建材
- 时装盔甲重置版（Cosmetic Armor Reworked）：提供免费的护甲和饰品外观。免费是指RLCraft有一套消耗素材修改护甲外观的机制，为了不牺牲RLCraft本身的趣味建议不加入，或者仅用于修改饰品外观
- 区块预生成器（Chunk-Pregenerator）：提前生成世界，冒险时快速探索世界生成区块会占用很多性能。
- 旅行者背包（Traveler's Backpack）：终极背包解决方案。RLCraft的背包管理对于仓鼠党来说比较头疼，如果追求舒适可以增加一个大背包。建议作为毕业科技的内容。与墓碑等模组兼容性不好。不推荐
- 旅行地图（Journey Map）：小地图。RLCraft自带更符合主题的古式地图（Antique Atlas），所以不推荐加入各种小地图
- Dynmap：世界地图。服务器展示世界或者单机世界用于展示时可以考虑，也提供网页－游戏聊天和标点等功能。如果想要显示提前生成世界的轮廓，但是不给出地图的细节，即战争迷雾效果，可以先用org.dynmap.hdmap.TopoHDShader完整渲染地图，然后使用org.dynmap.hdmap.TexturePackHDShader正常更新渲染玩家探索范围

![img](https://i0.hdslb.com/bfs/article/a6463ca5e99ca44b4474cebec18cbca060001f7f.png@1256w_708h_!web-article-pic.webp)添加内容

# 开服相关

![img](https://i0.hdslb.com/bfs/article/0117cbba35e51b0bce5f8c2f6a838e8a087e8ee7.png@progressive.webp)

- RLCraft的正常游戏体验需要服务器设置（server.properties）以下内容：启用命令方块才能正常生成RLCraft结构中的特定村民；允许飞行防止玩家在飞行时被踢出服务器；取消游戏刻检测避免大型结构生成造成的卡顿关闭服务器；锁定困难难度保持RLCraft的正常平衡设定。

```javascript
enable-command-block=true
allow-flight=true
max-tick-time=-1
difficulty=3
```

- 建议使用区块预生成器（Chunk-Pregenerator）提前生成世界。RLCraft默认生成器的世界尺寸是原版的4倍，并且玩家出生范围是出生点最大10000m的范围。冒险时快速探索世界生成区块会占用很多性能。
- 多人联机时出现无法攻击冰与火之歌的火龙和冰龙的情况，需要删除ISeeDragons模组。