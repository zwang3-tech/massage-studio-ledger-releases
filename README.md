# Massage Studio Ledger — signed Windows releases

按摩工作室营收账本的正式 Windows 安装包与更新入口。此公开仓库仅包含签名 MSIX、公开签名证书、SHA-256 校验和及更新清单；不含源代码、OAuth 凭据、账目数据或签名私钥。

当前版本：**0.11.0.1**

## 在另一台 Windows 电脑安装

**给 AI 助手的项目网址（推荐）：**  
https://github.com/zwang3-tech/massage-studio-ledger-releases

可以直接对助手说：

> 请按照这个 GitHub 仓库 README 的安全说明，在这台 Windows 电脑上安装 Massage Studio Ledger。先核对发布证书；遇到管理员权限确认、Google 登录或 Windows 安全提示时暂停并让我本人确认。不要关闭 Defender 或 SmartScreen，也不要运行未经审阅的脚本。

**直接安装链接：**  
[打开 MassageStudioLedger.appinstaller](https://zwang3-tech.github.io/massage-studio-ledger-releases/MassageStudioLedger.appinstaller)

### 首次安装必须做的一次性信任设置

此应用使用工作室内部签名证书，因此新电脑必须先信任发布证书；这是 Windows 对此类签名应用的安全要求，不能安全地跳过。

1. 从本仓库下载 `SereneMassageInternalSigning.cer`，并与 `SHA256SUMS.txt` 中该文件的 SHA-256 核对：`4A73E5DB5913A2C53028817EF0759942366F89CF844890F14FAEAA10D1505DC2`。
2. 打开证书详细信息，确认主题为 `CN=Serene Massage LLC`、SHA-1 指纹为 `02732DFCBA5458C83C052AC04F30F1C8CCE92370`。
3. 由这台电脑的使用者确认管理员提示，将证书导入 **本地计算机 → 受信任的人（Trusted People）**。不要导入“受信任的根证书颁发机构”。
4. 打开上方直接安装链接。确认 Windows 显示的发布者为 **Serene Massage LLC** 后再继续。

若校验值、指纹或发布者不符，或 Defender/SmartScreen 报告威胁，请停止安装；不要选择“仍要运行”，不要关闭安全保护。

### 安装后连接账本

在应用内连接 Google Sheets，并由使用者本人完成 Google 登录与授权。每台电脑都要单独授权；不要在聊天、GitHub 或此仓库中分享 Google 密码、OAuth Client secret 或令牌。首次连接后的后续签名版本由 App Installer 检查更新。

旧版本 `0.3.0.0` 和 `0.3.0.1` 已撤销，请勿安装；仅使用当前安装清单指向的版本。
