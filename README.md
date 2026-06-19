# STS2 CustomLab

Language / 语言：[中文](#中文) | [English](#english)

---

## 中文

**STS2 CustomLab** 是一个用于《Slay the Spire 2》的轻量级实验室 Mod，可在战斗中快速构建并热更新当前测试环境。

### 功能说明

- 在战斗内浏览并添加卡牌到当前测试牌组。
- 在战斗内浏览并添加怪物到当前遭遇。
- 点击 **Save + hot swap** 后立即热更新当前战斗，无需重开运行。
- 点击 **Reload config** 可重新加载外部配置。
- 仓库仅包含运行 Mod 必需的三个组件，便于直接安装和分发。

### 文件说明

| 文件 | 作用 |
| --- | --- |
| `STS2_CustomLab.dll` | Mod 主运行程序集。 |
| `STS2_CustomLab.json` | Mod 加载器使用的清单 / 元数据文件。 |
| `STS2_CustomLab.config.json` | CustomLab 的运行配置文件。 |

### 安装方式

将本仓库中的三个文件复制到《Slay the Spire 2》的 Mod 目录：

```text
Slay the Spire 2 v0.102.0/mods/STS2_CustomLab/
```

目录结构应为：

```text
STS2_CustomLab/
|-- STS2_CustomLab.dll
|-- STS2_CustomLab.json
`-- STS2_CustomLab.config.json
```

### 示意图说明

#### 怪物构建器

通过 **Monster builder** 面板搜索、筛选并添加怪物。右侧区域展示当前战斗中的怪物列表，并提供数量调整和移除等控制。

![怪物构建器](docs/images/monster-browser-selected.png)

#### 牌组构建器

通过 **Deck builder** 面板浏览卡池，可按类型、稀有度、费用等条件筛选卡牌，并将选中的卡加入当前战斗牌组。

![牌组构建器](docs/images/deck-builder-selected.png)

#### 保存并热更新

修改牌组或怪物列表后点击 **Save + hot swap**，Mod 会立即重建当前战斗状态。左下角日志会显示已应用的卡牌数量和怪物替换结果。

![保存并热更新](docs/images/hot-swap-applied.png)

---

## English

**STS2 CustomLab** is a lightweight Slay the Spire 2 mod for quickly building and hot-swapping the current combat lab setup.

### What it does

- Browse and add cards to the current combat deck.
- Browse and add monsters to the current combat encounter.
- Apply changes immediately with **Save + hot swap**, without restarting the run.
- Reload external configuration with **Reload config**.
- Keep the test setup small and focused by shipping only the required runtime files.

### Included files

| File | Purpose |
| --- | --- |
| `STS2_CustomLab.dll` | Main mod runtime assembly. |
| `STS2_CustomLab.json` | Mod manifest / metadata used by the loader. |
| `STS2_CustomLab.config.json` | Runtime configuration for CustomLab. |

### Installation

Copy the three files in this repository into your Slay the Spire 2 mod folder:

```text
Slay the Spire 2 v0.102.0/mods/STS2_CustomLab/
```

Expected layout:

```text
STS2_CustomLab/
|-- STS2_CustomLab.dll
|-- STS2_CustomLab.json
`-- STS2_CustomLab.config.json
```

### Usage screenshots

#### Monster browser

Use the **Monster builder** panel to search, filter, and add monsters to the current combat. The right side shows the current monster list and per-monster controls.

![Monster browser](docs/images/monster-browser-selected.png)

#### Deck builder

Use the **Deck builder** panel to browse the card pool, filter by type / rarity / cost, and add selected cards to the current combat deck.

![Deck builder](docs/images/deck-builder-selected.png)

#### Save + hot swap result

After editing the deck or monster list, click **Save + hot swap** to rebuild the combat state immediately. The message area reports the applied deck and monster replacement result.

![Save and hot swap result](docs/images/hot-swap-applied.png)
