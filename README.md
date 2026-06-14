# My Notes - 复古风格个人记事本

一个具有复古日记本风格的个人记事网页，支持桌面端和移动端使用。

## 功能特性

- **笔记管理** - 新建、编辑、删除笔记，数据保存在 localStorage 中
- **日历筛选** - 左侧日历面板，按年/月筛选笔记
- **一键删除** - 批量选择并删除笔记
- **Tab 缩进** - 编辑笔记时支持 Tab 键缩进
- **恐龙动画** - 右侧循环播放小恐龙跳障碍物的 2D 动画
- **头像设置** - 右上角可自定义用户头像
- **数据持久化** - 关闭浏览器后数据不会丢失

## 视觉风格

- 仿旧纸张纹理背景（浅米黄底 + 纸张质感）
- 手写体字体（Caveat / ZCOOL KuaiLe）
- 笔记卡片带阴影和圆角，类似手写便签
- 打字机风格标题

## 项目结构

```
owner_web/
├── my_notes.html          # 桌面端网页（直接浏览器打开即可使用）
├── MyNotes.apk            # Android 安装包
├── mynotes-app/           # Capacitor 移动端项目
│   ├── www/               # 移动端网页源码
│   ├── android/           # Android 原生项目
│   ├── .github/           # GitHub Actions 自动构建 APK
│   ├── capacitor.config.json
│   └── package.json
└── .gitignore
```

## 使用方式

### 桌面端

直接用浏览器打开 `my_notes.html` 即可使用。

### 移动端

1. 将 `MyNotes.apk` 传输到 Android 手机
2. 在手机设置中允许安装未知来源应用
3. 安装并打开

### 自动构建 APK

项目配置了 GitHub Actions，推送到 main 分支时会自动构建 APK。在 Actions 页面的 Artifacts 中下载即可。

## 技术栈

- HTML / CSS / JavaScript
- localStorage 数据存储
- Capacitor（Web 转 Native App）
- GitHub Actions CI/CD
