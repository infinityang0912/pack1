# 出行清单

两个人共用的出行物品清单。单文件网页，数据存在各自手机浏览器的本地存储里，不上传服务器。

## 部署到 GitHub Pages

**1. 建仓库**

打开 https://github.com/new

- Repository name：`packlist`（或者随便一串字母，网址里会用到）
- 选 **Public**（免费账号的 Pages 只能从公开仓库发布）
- 点 Create repository

**2. 传文件**

仓库页面 → `Add file` → `Upload files` → 把这个文件夹里的 6 个文件全拖进去：

```
index.html      ← 必须
manifest.json   ← 加到主屏幕用
sw.js           ← 断网也能打开
icon-180.png    ← iPhone 主屏幕图标
icon-192.png
icon-512.png
robots.txt      ← 不让搜索引擎收录
```

拖完点绿色 `Commit changes`。

**3. 打开 Pages**

仓库 → `Settings` → 左侧 `Pages`

- Source：`Deploy from a branch`
- Branch：`main`，目录 `/ (root)`
- 点 `Save`

**4. 等 1–3 分钟**

回到 Pages 页面刷新，顶部会出现：

```
https://你的用户名.github.io/packlist/
```

这就是手机要打开的网址。

## 手机上怎么用

**iPhone（Safari）**

1. Safari 打开上面那个网址
2. 点底部「分享」→「添加到主屏幕」
3. 桌面会出现一个勾选图标，以后点它直接全屏打开

**安卓（Chrome）**

1. Chrome 打开网址
2. 右上角三点 →「添加到主屏幕」

## 两个人的数据怎么对齐

**每个人的清单都存在自己手机里**，服务器上只有代码。所以：

- 你整理好清单 → ☰ →「发给 TA」→ 复制那段文字 → 微信发她
- 她打开网址 → ☰ →「发给 TA」→ 切到「接收」→ 粘贴 → 载入
- 两边从现在起是同一份

之后各自勾各自的，出门前再对一次。

## 注意

- **别把那段同步文字发到群里**。那才是你的清单内容（谁拿了什么），网址本身没有你的数据。
- 网址是公开可访问的。别人打开看到的是一个全新的空清单，看不到你勾了什么、加了什么。
- 想改清单之后更新线上版本：直接覆盖仓库里的 `index.html` 即可，手机重新打开就是新的。
