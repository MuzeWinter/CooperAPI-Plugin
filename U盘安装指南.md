# U盘安装指南 — 本地插件市场

## 步骤

### 1. 复制到目标电脑
把整个 CooperAPI-Plugin-marketplace 文件夹从 U 盘拷贝到目标电脑，例如：
`
C:\Users\用户名\CooperAPI-Plugin-marketplace\
`

> ⚠️ 不要直接从 U 盘使用，先拷贝到本地硬盘。

### 2. 找到 Codex 配置文件

在目标电脑打开：
`
C:\Users\用户名\.codex\config.toml
`

如果没有这个文件，新建一个。

### 3. 添加以下配置

`	oml
[marketplaces.CooperAPI-Plugin]
source_type = "local"
source = "C:\\Users\\用户名\\CooperAPI-Plugin-marketplace"

# 按需启用需要的插件（示例启用 product-design 和 browser）
[plugins."product-design@CooperAPI-Plugin"]
enabled = true

[plugins."browser@CooperAPI-Plugin"]
enabled = true
`

> source 路径改成你实际存放的路径，Windows 路径中 \ 要写成 \\

### 4. 重启 Codex

重启后即可使用。输入 @Product Design help me get started 验证。

---

## 可用插件列表（16个，按需启用）

`	oml
[plugins."browser@CooperAPI-Plugin"]
enabled = true

[plugins."canva@CooperAPI-Plugin"]
enabled = true

[plugins."chrome@CooperAPI-Plugin"]
enabled = true

[plugins."computer-use@CooperAPI-Plugin"]
enabled = true

[plugins."creative-production@CooperAPI-Plugin"]
enabled = true

[plugins."data-analytics@CooperAPI-Plugin"]
enabled = true

[plugins."documents@CooperAPI-Plugin"]
enabled = true

[plugins."hyperframes@CooperAPI-Plugin"]
enabled = true

[plugins."investment-banking@CooperAPI-Plugin"]
enabled = true

[plugins."presentations@CooperAPI-Plugin"]
enabled = true

[plugins."product-design@CooperAPI-Plugin"]
enabled = true

[plugins."public-equity-investing@CooperAPI-Plugin"]
enabled = true

[plugins."sales@CooperAPI-Plugin"]
enabled = true

[plugins."slack@CooperAPI-Plugin"]
enabled = true

[plugins."spreadsheets@CooperAPI-Plugin"]
enabled = true

[plugins."ui-ux-pro-max@CooperAPI-Plugin"]
enabled = true
`

> 不需要的插件不用启用，不会占用资源。