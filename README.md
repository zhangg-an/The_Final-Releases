# The Final Windows 交付

本仓库仅用于发布 The Final 的 Windows 便携版，不包含项目源码、数据库业务数据、账号密码、Cookie、浏览器登录状态或历史任务。

## 下载最新版

进入仓库右侧的 **Releases**，打开标记为 **Latest** 的版本，下载：

- `TheFinal-v<版本号>-Windows-x64.zip`
- 同名的 `.sha256.txt` 校验文件

请完整解压 ZIP 后，再双击文件夹内的 `TheFinal.exe`。不要直接在压缩包中运行，也不要只复制 EXE；程序所需的运行库位于同一文件夹中。

## 首次使用

1. 支持 Windows 10/11 x64。
2. 电脑需要安装 Google Chrome，并保持网络可用。
3. 将解压后的完整文件夹放到桌面或“文档”等当前用户有写入权限的位置。
4. 双击 `TheFinal.exe`，稍候应用会在默认浏览器打开。
5. 店小秘和 GIGA 首次使用时，需要由使用者本人在弹出的 Chrome 窗口中安全登录。
6. 应用数据保存在程序目录的 `data` 文件夹；升级前请先备份该文件夹。

详细说明请查看仓库中的 `使用说明.txt`。

## 版本规则

版本号采用语义化版本：

- `v1.0.1`：兼容性修复或小问题修复
- `v1.1.0`：新增向后兼容的功能
- `v2.0.0`：包含不兼容调整的大版本

每次更新都会建立新的 GitHub Release。用户可始终从 **Releases → Latest** 下载最新版，旧版本仍保留用于回退。

## 安全校验

下载后可在 PowerShell 中计算 SHA-256：

```powershell
Get-FileHash .\TheFinal-v1.4.0-Windows-x64.zip -Algorithm SHA256
```

结果应与 Release 中同名 `.sha256.txt` 文件一致。
