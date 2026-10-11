# 3D Sway — Product Site

After Effects 飘带形变插件 **3D Sway** 的产品官网（单页静态站点）。

## 内容

```
index.html          页面本体（单文件，样式与脚本内联）
assets/             页面配图与动效 GIF
assets/gallery/     场景画廊动效（30 段 + 6 组参数对比）
downloads/          插件下载包
downloads/3DSway-<版本>.zip
```

## 本地预览

页面使用相对路径引用资源，任意静态服务器即可：

```bash
python -m http.server 8080
```

然后访问 http://localhost:8080/

> 直接用 `file://` 打开也可正常显示，但 GIF 加载与跳转锚点的表现不如通过服务器访问可靠。

## 部署

推送到 `master` 分支后，GitHub Actions 自动发布到 GitHub Pages（见 `.github/workflows/pages.yml`）。

站点根目录即本仓库根目录，`index.html` 位于根路径。

## 相关仓库

插件源码、浏览器版引擎与素材预览库位于主仓库 `sway`，不在本仓库范围内。
