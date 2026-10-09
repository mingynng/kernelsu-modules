# KernelSU 模块仓库

这是一个替代官方 `modules.kernelsu.org` 的自定义模块仓库。

## 文件结构

```
kernelsu-module-repo/
├── modules.json      # 模块列表
├── README.md         # 本文件
└── .github/
    └── workflows/
        └── deploy.yml  # GitHub Pages 自动部署
```

## 部署方法

### 1. 创建 GitHub 仓库

在 GitHub 上新建一个仓库，比如叫 `kernelsu-modules`

### 2. 上传文件

把 `modules.json` 上传到仓库根目录

### 3. 开启 GitHub Pages

- 仓库 Settings → Pages
- Source 选择 `Deploy from a branch`
- Branch 选择 `main`，目录选 `/ (root)`
- 保存

### 4. 获取仓库地址

部署完成后，你的模块仓库地址就是：
`https://你的用户名.github.io/kernelsu-modules/modules.json`

## 修改 APK 的 URL

### 方法一：使用 APK 编辑器（推荐）

1. 下载 MT 管理器或 NP 管理器（手机上用）
2. 打开 KowSU Pro APK
3. 找到 `classes.dex` 文件
4. 搜索 `modules.kernelsu.org`
5. 替换成你的 GitHub Pages 地址
6. 保存并重新签名

### 方法二：使用 apktool（电脑上用）

```bash
# 反编译
apktool d KowSU\ Pro.apk

# 搜索并替换 URL
grep -rl "modules.kernelsu.org" smali/
sed -i 's/modules.kernelsu.org/你的用户名.github.io\/kernelsu-modules/g' smali/**/*.smali

# 重新打包
apktool b KowSU\ Pro -o KowSU\ Pro\ Modded.apk

# 签名
apksigner sign --ks my.keystore KowSU\ Pro\ Modded.apk
```

## 模块列表格式

`modules.json` 是一个 JSON 数组，每个模块的字段：

| 字段 | 说明 |
|------|------|
| moduleId | 模块唯一 ID |
| name | 模块名称 |
| version | 版本号 |
| versionCode | 版本代码（数字） |
| author | 作者 |
| description | 详细描述 |
| summary | 简短描述 |
| downloadUrl | 下载地址 |
| icon | 图标 URL |
| homepageUrl | 主页地址 |
| readme | README 地址 |

## 添加新模块

编辑 `modules.json`，在数组里添加新的模块对象即可。
