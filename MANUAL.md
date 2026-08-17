# AnZhiyu 主题配置文档

本文档基于 `_config.anzhiyu.yml` 配置文件，详细介绍 AnZhiyu 主题的各项配置选项。从基础设置到高级功能，帮助你全面定制自己的博客。

---

## 目录

1. [基础配置](#基础配置)
   - [菜单配置](#菜单配置)
   - [导航栏配置](#导航栏配置)
   - [哀悼日设置](#哀悼日设置)
   - [代码块设置](#代码块设置)
   - [复制版权设置](#复制版权设置)
   - [社交链接](#社交链接)
   - [作者卡片状态](#作者卡片状态)
   - [搜索功能](#搜索功能)
   - [数学公式](#数学公式)
   - [图片相关](#图片相关)
2. [文章相关配置](#文章相关配置)
   - [文章元数据](#文章元数据)
   - [主色调](#主色调)
   - [字数统计](#字数统计)
   - [首页文章摘要](#首页文章摘要)
   - [锚点](#锚点)
   - [文章目录](#文章目录)
   - [文章版权](#文章版权)
   - [打赏](#打赏)
   - [文章编辑链接](#文章编辑链接)
   - [相关文章](#相关文章)
   - [图片描述](#图片描述)
   - [文章分页](#文章分页)
   - [过期提醒](#过期提醒)
3. [分享与评论](#分享与评论)
   - [分享功能](#分享功能)
   - [评论系统](#评论系统)
4. [聊天服务](#聊天服务)
5. [页脚配置](#页脚配置)
   - [页脚所有者](#页脚所有者)
   - [运行时间](#运行时间)
   - [徽标列表](#徽标列表)
   - [社交栏](#社交栏)
   - [页脚链接列表](#页脚链接列表)
   - [页脚底部栏](#页脚底部栏)
6. [统计与分析](#统计与分析)
7. [广告](#广告)
8. [站长验证](#站长验证)
9. [美化与效果](#美化与效果)
   - [主题色](#主题色)
   - [移动端侧边栏](#移动端侧边栏)
   - [文章h2分隔线](#文章h2分隔线)
   - [表格隔行变色](#表格隔行变色)
   - [首页双栏显示](#首页双栏显示)
   - [首页顶栏设置](#首页顶栏设置)
   - [分类/标签页UI](#分类标签页ui)
   - [页脚背景](#页脚背景)
   - [右下角按钮位置](#右下角按钮位置)
   - [背景特效](#背景特效)
   - [打字效果](#打字效果)
   - [点击效果](#点击效果)
   - [显示模式](#显示模式)
   - [全局字体](#全局字体)
   - [博客标题字体](#博客标题字体)
   - [水平分隔线图标](#水平分隔线图标)
   - [主页副标题](#主页副标题)
   - [加载动画](#加载动画)
10. [侧边栏配置](#侧边栏配置)
    - [侧边栏通用设置](#侧边栏通用设置)
    - [作者卡片](#作者卡片)
    - [公告卡片](#公告卡片)
    - [微信卡片](#微信卡片)
    - [最近文章卡片](#最近文章卡片)
    - [分类卡片](#分类卡片)
    - [标签卡片](#标签卡片)
    - [归档卡片](#归档卡片)
    - [站点信息卡片](#站点信息卡片)
11. [访问统计与运行时间](#访问统计与运行时间)
    - [不蒜子统计](#不蒜子统计)
    - [运行时间显示](#运行时间显示)
12. [最新评论](#最新评论)
13. [右下角按钮](#右下角按钮)
    - [简繁转换](#简繁转换)
    - [阅读模式](#阅读模式)
    - [中控台](#中控台)
    - [深色模式](#深色模式)
    - [右侧项顺序](#右侧项顺序)
14. [图片灯箱](#图片灯箱)
15. [标签外挂](#标签外挂)
    - [Mermaid](#mermaid)
    - [Note 提示块](#note-提示块)
16. [图标库](#图标库)
17. [其他功能](#其他功能)
    - [Pjax](#pjax)
    - [Aplayer 注入](#aplayer-注入)
    - [Snackbar 弹窗](#snackbar-弹窗)
    - [Instant.page 预加载](#instantpage-预加载)
    - [Pangu.js 中英文空格](#pangujs-中英文空格)
    - [图片懒加载](#图片懒加载)
    - [PWA](#pwa)
    - [Open Graph 元标签](#open-graph-元标签)
    - [CSS 前缀](#css-前缀)
18. [首页顶部配置](#首页顶部配置)
    - [基础信息](#基础信息)
    - [分类快捷入口](#分类快捷入口)
    - [Banner 区域](#banner-区域)
    - [Swiper 轮播](#swiper-轮播)
19. [朋友圈配置](#朋友圈配置)
20. [深色模式粒子效果](#深色模式粒子效果)
21. [控制台打印](#控制台打印)
22. [51la 统计](#51la-统计)
23. [标签卖萌](#标签卖萌)
24. [留言弹幕](#留言弹幕)
25. [左下角音乐播放器](#左下角音乐播放器)
26. [音乐页面默认歌单](#音乐页面默认歌单)
27. [评论匿名邮箱](#评论匿名邮箱)
28. [文章底部工具](#文章底部工具)
29. [欢迎语](#欢迎语)
30. [文章顶部 AI 摘要](#文章顶部-ai-摘要)
31. [快捷键](#快捷键)
32. [无障碍优化](#无障碍优化)
33. [友情链接顶部配置](#友情链接顶部配置)
34. [缩略图后缀](#缩略图后缀)
35. [隐私协议弹窗](#隐私协议弹窗)
36. [右键菜单](#右键菜单)
37. [People Canvas 模式](#people-canvas-模式)
38. [动效配置](#动效配置)
39. [自定义代码注入](#自定义代码注入)
40. [CDN 配置](#cdn-配置)

---

## 基础配置

### 菜单配置

```yaml
menu:
  我的博客:
    归档: /archives/ || anzhiyu-icon-box-archive
    分类: /categories/ || anzhiyu-icon-shapes
    标签: /tags/ || anzhiyu-icon-tags
  友链和留言:
    友人帐: /link/ || anzhiyu-icon-link
    # 朋友圈: /fcircle/ || anzhiyu-icon-artstation
    留言板: /comments/ || anzhiyu-icon-envelope
  # 我的:
  #   音乐馆: /music/ || anzhiyu-icon-music
  #   追番页: /bangumis/ || anzhiyu-icon-bilibili
  #   相册集: /album/ || anzhiyu-icon-images
  #   小空调: /air-conditioner/ || anzhiyu-icon-fan
  关于:
    关于本人: /about/ || anzhiyu-icon-paper-plane
    # 闲言碎语: /essay/ || anzhiyu-icon-lightbulb
    随便逛逛: javascript:toRandomPost() || anzhiyu-icon-shoe-prints1
```

定义导航菜单项。每个菜单项包含显示名称、链接和图标类。支持二级菜单（如“我的博客”下有三个子项）。注释掉的项可取消注释启用。

### 导航栏配置

```yaml
nav:
  enable: false
  travelling: true
  clock: true
  menu:
    - title: 工程
      item:
        - name: TouchFish
          link: https://icc.gt.tc/touchfish
          icon: https://touchfish.ilovescratch.us.ci/logo.png
```

顶部导航栏（在菜单上方）。`enable` 控制是否启用。`travelling` 和 `clock` 控制是否显示旅行模式和时钟。`menu` 定义导航栏下拉菜单。

### 哀悼日设置

```yaml
mourn:
  enable: true
  days: [4-5, 5-12, 7-7, 9-18, 12-13]
```

在指定日期（月-日）将网站首页变灰（不包括滚动条）。可添加多个日期。

### 代码块设置

```yaml
highlight_theme: light
highlight_copy: true
highlight_lang: true
highlight_shrink: false
highlight_height_limit: 330
code_word_wrap: false
```

- `highlight_theme`：代码高亮主题，可选 `darker / pale night / light / ocean / mac / mac light / false`。
- `highlight_copy`：是否显示复制按钮。
- `highlight_lang`：是否显示代码语言。
- `highlight_shrink`：是否默认收缩代码块，`false` 展开，`true` 收缩，`none` 展开且隐藏按钮。
- `highlight_height_limit`：代码块高度限制（px），超出显示滚动条。
- `code_word_wrap`：是否自动换行。

### 复制版权设置

```yaml
copy:
  enable: true
  copyright:
    enable: false
    limit_count: 50
```

`enable`：复制后是否弹窗提示版权信息。`copyright`：复制内容后是否追加版权信息，`limit_count` 为触发版权信息的最小字符数。

### 社交链接

```yaml
social:
  Github: https://github.com/JohnChiao75 || anzhiyu-icon-github
  Email: mailto://johnchiao@outlook.com || anzhiyu-icon-envelope
```

格式：`名称: 链接 || 图标类`。用于显示在页面指定位置。

### 作者卡片状态

```yaml
author_status:
  enable: false
  statusImg: "https://cdn.luogu.com.cn/upload/usericon/1366636.png"
  skills:
    - Python 工程
    - OI
    - HTML/Electron 开发
```

侧边栏作者卡片中的状态显示（图片和技能列表）。需 `aside.card_author.enable` 配合。

### 搜索功能

支持三种搜索：

- **Algolia**：`algolia_search`，需配置 `hits.per_page` 等。
- **Docsearch**：`docsearch`，需申请 Algolia 账号并填写 `appId`, `apiKey`, `indexName`。
- **本地搜索**：`local_search`，`enable` 和 `preload` 控制是否启用和预加载。

### 数学公式

- **MathJax**：`mathjax`，需在文章 Front-matter 添加 `mathjax: true`。
- **KaTeX**：`katex`，`per_page: true` 表示所有页面加载，`false` 需手动添加 `mathjax: true`。

### 图片相关

- **Favicon**：`favicon` 网站图标。
- **头像**：`avatar.img` 头像图片，`effect` 是否启用头像特效。
- **顶部图片**：`disable_top_img` 禁用所有 banner 图；`index_img` 首页 banner；`default_top_img` 默认 banner。
- **文章封面**：`cover` 控制封面显示位置和默认封面。
- **错误图片替换**：`error_img` 友情链接和文章页加载失败时显示的图片。
- **404页面**：`error_404` 启用自定义 404 页。

## 文章相关配置

### 文章元数据

```yaml
post_meta:
  page:
    date_type: created
    date_format: simple
    categories: true
    tags: true
    label: false
  post:
    date_type: both
    date_format: date
    categories: true
    tags: true
    label: true
    unread: false
```

控制首页和文章页显示的元信息（日期、分类、标签等）。`date_type` 可选 `created`（创建日）、`updated`（更新日）、`both`。`date_format` 可选 `date`（具体日期）、`relative`（相对时间）、`simple`（简单格式）。

### 主色调

```yaml
mainTone:
  enable: false
  mode: api
  api: https://img2color-go.vercel.app/api?img=
  cover_change: true
```

从文章封面图提取主色调，用于页面主题色。`mode` 可选 `colorthief`（前端）、`cdn`（图片服务）、`api`（后端API）、`both`。可在文章 Front-matter 手动指定 `main_color`。

### 字数统计

```yaml
wordcount:
  enable: true
  post_wordcount: true
  min2read: true
  total_wordcount: true
```

启用后显示文章字数、阅读时长、站点总字数。

### 首页文章摘要

```yaml
index_post_content:
  method: 3
  length: 500
```

`method`：1 使用描述，2 描述+自动摘要，3 自动摘要。`length` 摘要长度。

### 锚点

```yaml
anchor: false
```

滚动时根据标题 ID 更新 URL。

### 文章目录

```yaml
toc:
  post: true
  page: false
  number: true
  expand: false
  style_simple: false
```

文章页和独立页是否显示目录，是否显示编号，是否展开全部层级，简单样式。

### 文章版权

```yaml
post_copyright:
  enable: true
  decode: false
  author_href:
  location: jsc'home
  license: CC BY-NC-SA 4.0
  license_url: https://creativecommons.org/licenses/by-nc-sa/4.0/
  avatarSinks: true
  copyright_author_img_back: /favicon.png
  copyright_author_img_front: /favicon.png
  copyright_author_link: /
```

文章底部版权声明，可自定义作者链接、协议等。

### 打赏

```yaml
reward:
  enable: false
```

文章底部打赏按钮，需自行配置二维码。

### 文章编辑链接

```yaml
post_edit:
  enable: true
  github: https://github.com/JohnChiao75/blog-new/edit/master/source/
  yuque: false
```

在文章页显示“编辑”链接，可跳转到 GitHub 或语雀编辑源文件。

### 相关文章

```yaml
related_post:
  enable: true
  limit: 6
  date_type: created
```

显示与当前文章相关的文章，基于标签等。

### 图片描述

```yaml
photofigcaption: false
```

是否在图片下方显示 `figcaption`。

### 文章分页

```yaml
post_pagination: 2
```

- `1`：下一篇为旧文章。
- `2`：下一篇为新文章。
- `3`/`4`：滚动到评论区时显示下一篇（带封面/不带）。
- `false`：禁用。

### 过期提醒

```yaml
noticeOutdate:
  enable: false
  style: flat
  limit_day: 365
  position: top
  message_prev: It has been
  message_next: days since the last update, the content of the article may be outdated.
```

文章更新超过指定天数后，在顶部或底部显示提醒。

## 分享与评论

### 分享功能

```yaml
addtoany:
  enable: true
  item: wechat,email,copy_link,qzone,print
```

使用 AddToAny 分享服务，可自定义显示的分享按钮。

### 评论系统

```yaml
comments:
  use: giscus
  text: true
  lazyload: true
  count: true
  card_post_count: true
```

支持 Valine/Waline/Twikoo/Artalk/giscus。`use` 选择使用的评论系统。下方有对应评论系统的详细配置项（如 `giscus` 需要 `repo`, `repo_id`, `category_id` 等）。`lazyload` 滚动到评论区域才加载，`count` 显示评论数。

## 聊天服务

```yaml
chat_btn: true
chat_hide_show: true
chatra:
  enable: true
  id: thYTgbqQiKrPT4ReZ
tidio:
  enable: false
  public_key:
...
```

聊天按钮开关及具体服务配置（chatra, tidio, daovoice, crisp）。

## 页脚配置

### 页脚所有者

```yaml
footer:
  owner:
    enable: true
    since: 2026
```

显示版权年份和作者。

### 运行时间

```yaml
runtime:
  enable: false
  launch_time: 04/01/2021 00:00:00
  work_img: ...
  work_description: ...
  offduty_img: ...
  offduty_description: ...
```

显示网站已运行时间，可设置上班/下班状态图片和描述。

### 徽标列表

```yaml
bdageitem:
  enable: false
  list:
    - link: https://hexo.io/
      shields: https://npm.elemecdn.com/anzhiyu-blog@2.1.5/img/badge/Frame-Hexo.svg
      message: 博客框架为Hexo_v5.4.0
```

使用 shields.io 风格的徽标，可链接到指定网站。

### 社交栏

```yaml
socialBar:
  enable: true
  centerImg:
  left:
    - title: Email
      link: mailto:johnchiao@outlook.com
      icon: anzhiyu-icon-envelope
  right:
    - title: CC
      link: /copyright
      icon: anzhiyu-icon-copyright-line
```

页脚左右两侧的社交图标。

### 页脚链接列表

```yaml
list:
  enable: false
  randomFriends: 3
  project:
    - title: 服务
      links:
        - title: 51la统计
          link: https://v6.51.la/
```

在页脚显示多列链接，可设置随机友链数量。

### 页脚底部栏

```yaml
footerBar:
  enable: true
  authorLink: /
  cc:
    enable: false
    link: /copyright
  linkList:
    - link: https://github.com/anzhiyu-c/hexo-theme-anzhiyu
      text: 主题
  subTitle:
    enable: true
    effect: true
    startDelay: 300
    typeSpeed: 150
    backSpeed: 50
    loop: false
    source: 1
    sub:
      - 生活明朗&#44; 万物可爱&#44; 人间值得&#44; 未来可期.
```

页脚最底部的版权链接和打字效果副标题。`source` 可调用第三方句子 API（1 一言，2 一句网，3 今日诗词）。

## 统计与分析

支持百度统计、Google Analytics、CNZZ、Cloudflare、Microsoft Clarity。填写对应的 ID 即可。

## 广告

```yaml
google_adsense:
  enable: false
  auto_ads: true
  js: https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js
  client:
  enable_page_level_ads: true
```

Google AdSense 配置。也可手动插入广告（`ad` 字段）。

## 站长验证

```yaml
site_verification:
  - name: google-site-verification
    content: xxx
  - name: baidu-site-verification
    content: code-xxx
```

用于搜索引擎站长验证。

## 美化与效果

### 主题色

```yaml
theme_color:
  enable: true
  main: "#425AEF"
  dark_main: "#3fe0f0"
  paginator: "#425AEF"
  ...
```

自定义各种场景下的颜色，需用双引号包裹。

### 移动端侧边栏

```yaml
sidebar:
  site_data:
    archive: true
    tag: true
    category: true
  menus_items: true
  tags_cloud: true
  display_mode: true
  nav_menu_project: true
```

控制移动端侧边栏显示哪些模块。

### 文章h2分隔线

```yaml
h2Divider: false
```

是否在文章 h2 标题下添加分隔线。

### 表格隔行变色

```yaml
table_interlaced_discoloration: false
```

表格偶数行背景色不同。

### 首页双栏显示

```yaml
article_double_row: true
```

首页文章列表以双栏网格显示。

### 首页顶栏设置

```yaml
index_site_info_top:
index_top_img_height:
```

自定义首页站点信息距离顶部距离和 top_img 高度。

### 分类/标签页UI

```yaml
category_ui:
tag_ui:
```

留空则与归档页相同，设为 `index` 则与首页相同。

### 页脚背景

```yaml
footer_bg: false
```

是否显示页脚背景图。

### 右下角按钮位置

```yaml
rightside-bottom: 100px
```

右下角按钮距离底部的距离。

### 背景特效

- `canvas_ribbon`：静止彩带。
- `canvas_fluttering_ribbon`：动态彩带。
- `canvas_nest`：线条网络。
- `universe`：深色模式粒子效果（独立配置，见后）。

### 打字效果

```yaml
activate_power_mode:
  enable: true
  colorful: true
  shake: false
  mobile: true
```

打字时出现粒子特效，类似“激活 power mode”。

### 点击效果

- `fireworks`：点击烟火。
- `click_heart`：点击爱心。
- `ClickShowText`：点击显示文字。

### 显示模式

```yaml
display_mode: light
```

默认亮色/暗色模式。

### 全局字体

```yaml
font:
  global-font-size: 16px
  code-font-size:
  font-family:
  code-font-family: consolas, Menlo, "PingFang SC", "Microsoft JhengHei", "Microsoft YaHei", sans-serif
```

设置全局字体和代码字体。

### 博客标题字体

```yaml
blog_title_font:
  font_link:
  font-family: PingFang SC, 'Hiragino Sans GB', 'Microsoft JhengHei', 'Microsoft YaHei', sans-serif
```

左上角和主页中心的标题字体。

### 水平分隔线图标

```yaml
hr_icon:
  enable: true
  icon: \f0c4
  icon-top:
```

在 `<hr>` 处显示 Font Awesome 图标，`icon` 为 unicode 值。

### 主页副标题

```yaml
subtitle:
  enable: true
  effect: true
  startDelay: 300
  typeSpeed: 150
  backSpeed: 50
  loop: true
  source: 1
  sub:
    - 生活明朗&#44;万物可爱&#44;人间值得&#44;未来可期.
```

主页打字副标题，可调用第三方句子 API。

### 加载动画

```yaml
preloader:
  enable: true
  source: 3
  pace_css_url:
  avatar: https://cdn.luogu.com.cn/upload/usericon/1366636.png
```

`source` 可选 `1`（全屏加载）、`2`（进度条）、`3`（自定义头像动画）。

## 侧边栏配置

### 侧边栏通用设置

```yaml
aside:
  enable: true
  hide: false
  button: true
  mobile: true
  position: left
  display:
    archive: true
    tag: true
    category: true
```

全局启用侧边栏，可设置移动端显示、位置、哪些页面显示。

### 作者卡片

```yaml
card_author:
  enable: true
  description: ...
  name_link: /
```

显示作者头像、简介。`description` 支持 HTML。

### 公告卡片

```yaml
card_announcement:
  enable: true
  content: 欢迎来看我的博客鸭~
```

简单的公告文字。

### 微信卡片

```yaml
card_weixin:
  enable: false
  face: ...
  backFace: ...
```

显示微信公众号二维码，可正反面切换。

### 最近文章卡片

```yaml
card_recent_post:
  enable: true
  limit: 5
  sort: date
```

显示最近文章数量，按日期排序。

### 分类卡片

```yaml
card_categories:
  enable: true
  limit: 8
  expand: none
```

显示分类列表，`expand` 控制是否展开子分类。

### 标签卡片

```yaml
card_tags:
  enable: true
  limit: 40
  color: false
  highlightTags:
    # - Hexo
```

显示标签云，可高亮某些标签。

### 归档卡片

```yaml
card_archives:
  enable: true
  type: monthly
  format: MMMM YYYY
  order: -1
  limit: 8
```

按月或年归档文章。

### 站点信息卡片

```yaml
card_webinfo:
  enable: true
  post_count: true
  last_push_date: false
```

显示文章总数、最后更新日期等。

## 访问统计与运行时间

### 不蒜子统计

```yaml
busuanzi:
  site_uv: true
  site_pv: true
  page_pv: true
```

显示站点 UV/PV 和页面 PV。

### 运行时间显示

```yaml
runtimeshow:
  enable: true
  publish_date: 4/1/2021 00:00:00
```

显示网站已运行时间。

## 最新评论

```yaml
newest_comments:
  enable: true
  limit: 6
  storage: 10
  avatar: true
```

在侧边栏显示最新评论，可缓存到 localStorage。

## 右下角按钮

### 简繁转换

```yaml
translate:
  enable: false
  default: 繁
  rightMenuMsgDefault: "轉為繁體"
  ...
```

开启后右下角出现简繁转换按钮，可自定义文字。

### 阅读模式

```yaml
readmode: true
```

启用阅读模式按钮，点击后隐藏侧边栏等，优化阅读体验。

### 中控台

```yaml
centerConsole:
  enable: true
  card_tags:
    enable: true
    limit: 40
  card_archives:
    enable: true
    type: monthly
    format: MMMM YYYY
    order: -1
    limit: 8
```

中控台（右下角控制面板）显示标签和归档卡片。

### 深色模式

```yaml
darkmode:
  enable: true
  button: true
  autoChangeMode: 1
  start:
  end:
```

深色模式开关，`autoChangeMode` 自动切换：1 跟随系统，2 固定时间（6pm-6am）。可自定义开始结束时间。

### 右侧项顺序

```yaml
rightside_item_order:
  enable: false
  hide:
  show:
```

自定义右下角按钮的显示顺序和隐藏项。

## 图片灯箱

```yaml
medium_zoom: false
fancybox: true
```

二选一：`medium_zoom` 或 `fancybox`，用于点击图片放大查看。

## 标签外挂

### Mermaid

```yaml
mermaid:
  enable: true
  theme:
    light: default
    dark: dark
```

支持 Mermaid 流程图、时序图等。

### Note 提示块

```yaml
note:
  style: flat
  icons: true
  border_radius: 3
  light_bg_offset: 0
```

`note` 标签的样式，可选 `simple`、`modern`、`flat`、`disabled`。

## 图标库

```yaml
icons:
  ali_iconfont_js: # 阿里图标symbol 引用链接
  fontawesome: false
  fontawesome_animation_css:
```

可引入阿里图标库 symbol 链接，或启用 Font Awesome 6。

## 其他功能

### Pjax

```yaml
pjax:
  enable: true
  exclude:
    # - xxxx
```

启用 Pjax 实现无刷新加载，可排除某些链接。

### Aplayer 注入

```yaml
aplayerInject:
  enable: true
  per_page: true
```

全局注入 Aplayer 播放器所需 JS/CSS。

### Snackbar 弹窗

```yaml
snackbar:
  enable: true
  position: top-center
  bg_light: "#425AEF"
  bg_dark: "#1f1f1f"
```

复制成功等操作的提示弹窗。

### Instant.page 预加载

```yaml
instantpage: true
```

鼠标悬停链接时预加载页面。

### Pangu.js 中英文空格

```yaml
pangu:
  enable: true
  field: site
```

自动在中英文之间插入空格，`field` 可选 `site`（全局）或 `post`（仅文章）。

### 图片懒加载

```yaml
lazyload:
  enable: true
  field: site
  placeholder:
  blur: true
  progressive: true
```

图片懒加载，可设置占位图、模糊效果。

### PWA

```yaml
pwa:
  enable: true
  startup_image_enable: true
  manifest: /manifest.json
  theme_color: var(--anzhiyu-main)
  ...
```

启用 PWA，配置 manifest 和图标路径。

### Open Graph 元标签

```yaml
Open_Graph_meta: true
```

为社交媒体分享生成 Open Graph 标签。

### CSS 前缀

```yaml
css_prefix: true
```

自动添加 CSS 浏览器前缀（如 `-webkit-`）。

## 首页顶部配置

### 基础信息

```yaml
home_top:
  enable: true
  timemode: date
  title: 生活明朗
  subTitle: 万物可爱。
  siteText: johnch.us.ci
  default_descr: 再怎么看我也不知道怎么描述它的啦！
```

首页顶部区域显示的标题、副标题、站点文本等。

### 分类快捷入口

```yaml
category:
  - name: 工程
    path: /categories/工程/
    shadow: var(--anzhiyu-shadow-blue)
    class: blue
    icon: anzhiyu-icon-dove
```

显示几个分类卡片，点击跳转。

### Banner 区域

```yaml
banner:
  tips: WELCOME
  title: 欢迎来到我的 Blog
  image: https://pic4.zhimg.com/v2-c34c61a90095abb8713de9d1dca7ec7b_r.jpg
  link: /
```

首页大图区域，可带链接。

### Swiper 轮播

```yaml
swiper:
  enable: false
  swiper_css: ...
  swiper_js: ...
```

若启用，可自定义 Swiper 库 CDN。

## 朋友圈配置

```yaml
friends_vue:
  enable: false
  vue_js: ...
  apiurl: ...
  top_tips: ...
  top_background:
```

用于显示友链朋友圈（友链最新文章），需后端支持。

## 深色模式粒子效果

```yaml
universe:
  enable: true
```

深色模式下显示粒子背景。

## 控制台打印

```yaml
console:
  enable: true
```

在浏览器控制台打印自定义信息。

## 51la 统计

```yaml
LA:
  enable: false
  ck:
  LingQueMonitorID:
```

51la 网站统计配置。

## 标签卖萌

```yaml
diytitle:
  enable: true
  leaveTitle: w(ﾟДﾟ)w 不要走！再看看嘛！
  backTitle: ♪(^∇^*)欢迎肥来！
```

当用户离开/返回标签页时修改页面标题。

## 留言弹幕

```yaml
comment_barrage_config:
  enable: false
  maxBarrage: 1
  barrageTime: 4000
  accessToken: ""
  mailMd5: ""
```

在评论区显示弹幕效果，需配置 token 和博主邮箱 MD5。

## 左下角音乐播放器

```yaml
nav_music:
  enable: false
  console_widescreen_music: false
  id: 8152976493
  server: netease
  volume: 0.7
  all_playlist: https://y.qq.com/n/ryqq/playlist/8802438608
```

左下角悬浮音乐播放器，支持网易云、QQ 音乐等。

## 音乐页面默认歌单

```yaml
music_page_default: nav_music
```

`/music` 页面默认加载 `nav_music` 配置的歌单，或 `custom` 自定义。

## 评论匿名邮箱

```yaml
visitorMail:
  enable: true
  mail: ""
```

可为未登录评论者统一设置一个匿名邮箱（用于 Gravatar 头像）。

## 文章底部工具

```yaml
ptool:
  enable: true
  share_mobile: true
  share_weibo: true
  share_copyurl: true
  categories: false
  mode:
```

文章底部显示的分享、复制链接、分类等工具。

## 欢迎语

```yaml
greetingBox:
  enable: true
  default: 晚上好👋
  list:
    - greeting: 晚安😴
      startTime: 0
      endTime: 5
    ...
```

根据时间段显示不同的欢迎语。

## 文章顶部 AI 摘要

```yaml
post_head_ai_description:
  enable: true
  gptName: AnZhiYu
  mode: local
  switchBtn: false
  btnLink: https://afdian.net/item/886a79d4db6711eda42a52540025c377
  randomNum: 3
  basicWordCount: 1000
  key: xxxx
  Referer: https://xx.xx/
```

文章开头显示 AI 生成的摘要，`mode` 可选 `tianli`（第三方服务）或 `local`（本地生成）。需配置 key 等。

## 快捷键

```yaml
shortcutKey:
  enable: true
  delay: 100
  shiftDelay: 200
```

启用快捷键，可设置延迟避免与浏览器冲突。

## 无障碍优化

```yaml
accesskey:
  enable: true
```

启用 accesskey 快捷键（按 `shift + ?` 查看帮助）。

## 友情链接顶部配置

```yaml
linkPageTop:
  enable: false
  title: 与数百名博主无限进步
  addFriendPlaceholder: "昵称（请勿包含博客等字样）：\n网站地址（要求博客地址，请勿提交个人主页）：\n..."
```

友链页面顶部标题和申请格式提示。

## 缩略图后缀

```yaml
pageThumbnailSuffix: ""
```

可为归档/标签/分类页的缩略图添加后缀（如 `-thumb`），用于调用不同尺寸图片。

## 隐私协议弹窗

```yaml
agreementPopup:
  enable: false
  url: /privacy
```

首次访问时弹窗显示隐私协议，点击跳转指定页面。

## 右键菜单

```yaml
rightClickMenu:
  enable: true
```

自定义右键菜单。

## People Canvas 模式

```yaml
peoplecanvas:
  enable: false
  img: https://upload-bbs.miyoushe.com/upload/2024/07/27/125766904/ba62475f396df9de3316a08ed9e65d86_5680958632268053399..png
```

首页“随便逛逛”模式切换为“人物行走”动画而非技能点。

## 动效配置

```yaml
dynamicEffect:
  postTopWave: true
  postTopRollZoomInfo: false
  pageCommentsRollZoom: false
```

文章顶部波浪效果、滚动缩放效果等。

## 自定义代码注入

```yaml
inject:
  head:
    # - <link rel="stylesheet" href="/css/custom.css" media="defer" onload="this.media='all'">
  bottom:
    # - <script src="/js/xxx"></script>
```

在 `</head>` 前和 `</body>` 前插入自定义 HTML/JS/CSS。

## CDN 配置

```yaml
CDN:
  internal_provider: local
  third_party_provider: cbd
  version: true
  custom_format: # https://npm.elemecdn.com/${name}@latest/${file}
  option:
    # main_css:
    # main:
    # ...
```

配置内部和第三方资源的 CDN 提供商，可选 `local`、`elemecdn`、`jsdelivr` 等。`option` 可单独覆盖某个资源的 CDN 链接。

---

本文档涵盖了 AnZhiYu 主题 `_config.anzhiyu.yml` 中的所有配置项。根据实际需求修改对应字段，重启 Hexo 服务器即可生效。部分功能需要额外安装插件或申请第三方服务，请参考主题官方文档。