# Stronghold-Protocol-Economy-Plugin · 数值调节插件

《明日方舟》「卫戍协议：盟约」同人复刻 [Stronghold-Protocol](https://github.com/sganggs/Stronghold-Protocol) 的**内容类插件**：只改两个数字——**场上部署人数上限**与**每回合发放的资金（含初始资金）**。

- 插件 id：`economy-knobs` · 版本 `1.0.1`
- 类型：**content（数据）插件**，无代码、不加干员、不加规则，通过一条数据补丁覆盖数值。
- 兼容：`app >=0.3.0 <0.5.0`，五个官方数据版本全支持。
- 权限：`data.patch`。装了它的房间对局标记为**非官方**。

## 安装

1. 把 `economy-knobs/` 整个文件夹复制到游戏根目录的 `plugins/` 下（文件夹名必须是插件 id）。
2. 重启服务器或刷新页面（下次扫描自动识别，**无需改任何本体文件**）。
3. 房主在房间「插件」面板勾选启用，全房间生效。

```bash
node tools/plugin.mjs list                 # 应看到 economy-knobs (loaded)
node tools/plugin.mjs check economy-knobs --strict
```

## 改数值

唯一需要编辑的文件：**`economy-knobs/knobs.json`**（标准数据补丁 `{patch:1, ops:[...]}`）。
详见插件内 [economy-knobs/README.md](economy-knobs/README.md)。

## 许可与署名

- 插件本身：**CC0-1.0**（见 [LICENSE](LICENSE)），可自由使用/修改/再分发。
- 运行它的引擎 [Stronghold-Protocol](https://github.com/sganggs/Stronghold-Protocol) 为 **GPL-3.0**，版权归原作者 sganggs；游戏素材版权归 上海鹰角网络 / Yostar，与本插件无关。
- 发布 / 维护：[TWCY114](https://github.com/TWCY114)。

非官方同人作品，仅供学习交流，严禁商用。
