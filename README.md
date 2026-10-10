# 湖山漫游记

给湖山的 25 岁生日礼物。坐上三猫小列车，在六角小岛上收集回忆、照片和祝福。

**[打开游戏](https://violetloveai.github.io/hushan-25-birthday/)** · [查看九个新人物彩蛋](https://violetloveai.github.io/hushan-25-birthday/personal-eggs.html)

![游戏中的湖山个人彩蛋](./preview.png)

## 怎么玩

- 点击列车旁亮起的六边格，一格算一步。首次到达回忆或彩蛋地点时，会自动打开故事。
- 在收藏册里查看照片、校园彩蛋和「湖山的小档案」，点击插画可放大。
- 走到第 25 步，拆开生日祝福，整张地图和全部照片随之开放。收藏册里的未读信封可以逐个揭晓，也可以一键全部揭开。

电脑和手机浏览器都能游玩。支持拖动与缩放地图、键盘操作和声音开关。每次进入都会开始新的漫游。

## 这一版

45 处地图发现：26 组照片回忆、10 处校园彩蛋、9 处湖山个人彩蛋。另有 5 个村庄奖励和生日终章。

相册收录 50 张图片：49 张照片和 1 张三猫头像。2026 年国庆旅行分成两组，分别保留。9 个个人彩蛋围绕专业、成绩、工作、家乡和爱好展开，新增 9 张人物插画和 9 张地图标记。

## 本地查看

本仓库保存已构建的静态网站，无需安装 npm 包或执行构建。安装 Git 和 Python 3 后，在终端依次运行：

```bash
git clone https://github.com/violetloveAI/hushan-25-birthday.git
cd hushan-25-birthday
python3 -m http.server 4175 --bind 127.0.0.1
```

随后打开 [本地游戏](http://127.0.0.1:4175/)。通过 HTTP 访问页面，浏览器才能正常加载模块。结束预览时，在终端按 `Ctrl+C`。

## 文件与部署

- `index.html`：游戏入口。
- `assets/`：Vite 构建的 JavaScript、CSS，以及字体和插画。
- `photos/`：网页照片与缩略图。
- `audio/`：背景音乐、音效及许可说明。
- `personal-eggs.html`：新增人物彩蛋的图片总览。

GitHub Pages 从 `main` 分支根目录发布。游戏为纯静态页面，没有账号、API 密钥或后端服务；运行所需的图片、字体和音频随网站提供。

发布仓库只保留网站使用的文件，不包含工程源码、原始 HEIC 照片、作图原始 PNG 或绘图提示词。

## 素材说明

本项目用于个人生日纪念。照片、个人内容和原创美术未授予复用许可。人物和地图插画使用内置 image_gen 生成；画面中的机构标记用于叙述个人经历，不代表机构参与或认可本项目。

第三方素材的来源和许可保留在仓库中：

- [字体来源](assets/fonts/SOURCES.txt)、[霞鹜文楷许可](assets/fonts/LXGW-LICENSE.txt)、[得意黑许可](assets/fonts/SMILEY-LICENSE.txt)
- [音乐与音效署名](audio/licenses/ATTRIBUTION.txt)、[CC BY 4.0](audio/licenses/CC-BY-4.0.txt)
- [音效详情](audio/sfx/ATTRIBUTION.txt)、[CC0](audio/sfx/licenses/CC0-1.0.txt)
