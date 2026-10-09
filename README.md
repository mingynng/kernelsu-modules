# KernelSU 模块仓库

这是一个自定义的 KernelSU 模块仓库，替代官方已下线的 `modules.kernelsu.org`。

## 仓库信息

- **模块数量**：18 个常用模块
- **更新时间**：2026-10-09
- **格式**：KernelSU 标准 modules.json
- **仓库地址**：`https://mingynng.github.io/kernelsu-modules/modules.json`

---

## 模块分类

### 🔒 隐藏环境（7个）
| 模块 | 说明 |
|------|------|
| Play Integrity Fix | 绕过 Play 完整性检测（游戏/支付/银行必装） |
| Tricky Store | 密钥认证绕过（配合 Play Integrity 使用） |
| Hide My Applist | 隐藏应用列表（防止应用扫描检测） |
| Shamiko | 隐藏 Root 环境（配合 Zygisk 使用） |
| Zygisk-Detach | 让应用从 Play 商店隐藏 |
| IAmNotADeveloper | 隐藏开发者选项状态 |
| CorePatch | Zygisk 核心补丁 |

### 🛠️ 基础框架（4个）
| 模块 | 说明 |
|------|------|
| Zygisk Next | Zygisk 兼容层（装 LSPosed 必装） |
| LSPosed | Xposed 框架（模块开发必备） |
| Magic OverlayFS | 元模块（修改系统文件必需） |
| CorePatch | Zygisk 核心补丁 |

### 🚀 性能优化（2个）
| 模块 | 说明 |
|------|------|
| MAGNETAR | 智能内核性能优化 |
| FunBox | 性能增强（温控/存储/网络优化） |

### 📱 功能增强（2个）
| 模块 | 说明 |
|------|------|
| Smart Pixels | Pixel 设备特性移植 |
| SystemUI Tuner | 系统 UI 高级自定义 |

### 🧰 实用工具（4个）
| 模块 | 说明 |
|------|------|
| AdAway | 全系统广告拦截 |
| NetProxy | 全系统代理设置 |
| DeviceID Changer | 修改设备 ID（防追踪） |
| MRepo | 第三方模块管理器（功能更强） |

---

## 使用方法

### 方法 1：在 KernelSU 管理器中添加
1. 打开 KernelSU 管理器
2. 进入「模块」页面
3. 添加自定义仓库 URL：
   ```
   https://mingynng.github.io/kernelsu-modules/modules.json
   ```

### 方法 2：手动下载安装
1. 在下方模块列表中找到需要的模块
2. 点击 GitHub 链接下载 zip 包
3. 在 KernelSU 管理器中选择「从本地安装」

---

## 模块列表

| ID | 名称 | 版本 | 作者 | 简介 |
|----|------|------|------|------|
| playintegrityfix | Play Integrity Fix | v19.2 | chiteroman, KOWX712 | 绕过 Play 完整性检测 |
| tricky_store | Tricky Store | v3.3.0 | 5ec1cff | 密钥认证绕过 |
| zygisk_next | Zygisk Next | v1.0.6 | Dr-TSNG | Zygisk 兼容层 |
| lsposed | LSPosed | v1.10.3 | LSPosed Team | Xposed 框架 |
| hide_my_applist | Hide My Applist | v3.5.2 | Dr-TSNG | 隐藏应用列表 |
| shamiko | Shamiko | v1.2.0 | LSPosed | 隐藏 Root 环境 |
| zygisk_detach | Zygisk-Detach | v0.6.5 | j-hc | Play 商店隐藏 |
| magic_overlayfs | Magic OverlayFS | v1.3.2 | KernelSU-Modules-Repo | 元模块 |
| adaway | AdAway | v6.1.0 | AdAway | 全系统广告拦截 |
| magnetar | MAGNETAR | v5.0.0 | magnetar-dev | 智能内核优化 |
| funbox | FunBox | v2.0.0 | funbox-dev | 性能增强 |
| smart_pixel | Smart Pixels | v1.7.0 | itsmalik030 | Pixel 特性移植 |
| systemui_tuner | SystemUI Tuner | v3.0.0 | zacharee | UI 自定义 |
| netproxy | NetProxy | v1.2.0 | KernelSU-Modules-Repo | 系统代理 |
| deviceid_changer | DeviceID Changer | v2.0.0 | KernelSU-Modules-Repo | 设备 ID 修改 |
| corepatch | CorePatch | v1.5.0 | LSPosed | Zygisk 补丁 |
| iamnotadeveloper | IAmNotADeveloper | v1.0.0 | various | 隐藏开发者选项 |
| mrepo | MRepo | v1.0.5 | MRepoApp | 第三方模块管理器 |

---

## 注意事项

- 本仓库仅收集公开模块，不提供任何破解/付费模块
- 请从官方 GitHub 下载最新版本
- 安装模块前请备份数据
- 如遇问题请前往对应模块的 GitHub 页面反馈

## 许可证

各模块版权归原作者所有。
