<div align="center">
  <img src="assets/banner.svg" alt="把数学和物理写成代码 — 魔方玩家 · 在读学生" width="100%">
</div>

<p align="center">
  <img src="https://img.shields.io/github/followers/JackPeng-Coder?style=flat-square&labelColor=0A0C10&color=3E63DD" alt="Followers">
  <img src="https://img.shields.io/github/stars/JackPeng-Coder?style=flat-square&labelColor=0A0C10&color=F2D024" alt="Stars">
  <img src="https://komarev.com/ghpvc/?username=JackPeng-Coder&style=flat-square&color=3E63DD&label=profile+views" alt="Profile views">
</p>

## 关于我

在读学生。写代码的偏好比较明显：比起做业务系统，我更喜欢把数学和物理里的东西变成能跑、能看、能玩的程序——分形渲染器、三体轨道、自研物理引擎、咖啡因在体内的代谢曲线。

魔方是我的另一条线。玩久了，顺手把这份爱好也写成了工具：模拟器、计时器数据互转、赛事监控。

技术上是个实用主义者：**Python** 用来快速验证想法，**TypeScript** 用来把想法做成界面，**C++** 用来刷题和抠性能。

## 技术栈

**语言**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)

**Web 与图形**

![Vue 3](https://img.shields.io/badge/Vue_3-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![WebGL2](https://img.shields.io/badge/WebGL2-990000?style=flat-square&logo=webgl&logoColor=white)
![WebRTC](https://img.shields.io/badge/WebRTC-333333?style=flat-square&logo=webrtc&logoColor=white)
![Express](https://img.shields.io/badge/Express-0A0C10?style=flat-square&logo=express&logoColor=white)
![PWA](https://img.shields.io/badge/PWA-5A0FC8?style=flat-square&logo=pwa&logoColor=white)

**桌面与科学计算**

![Pygame](https://img.shields.io/badge/Pygame-2E7D32?style=flat-square&logo=python&logoColor=white)
![PySide6](https://img.shields.io/badge/PySide6_·_QML-41CD52?style=flat-square&logo=qt&logoColor=white)
![Tkinter](https://img.shields.io/badge/Tkinter-3776AB?style=flat-square&logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Pillow](https://img.shields.io/badge/Pillow-3E63DD?style=flat-square&logo=python&logoColor=white)
![PyInstaller](https://img.shields.io/badge/PyInstaller-1F3A5F?style=flat-square&logo=python&logoColor=white)

**数据与工具**

![Flask](https://img.shields.io/badge/Flask-0A0C10?style=flat-square&logo=flask&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![BeautifulSoup](https://img.shields.io/badge/BeautifulSoup-43B02A?style=flat-square&logo=python&logoColor=white)
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=flat-square&logo=arduino&logoColor=white)

## 精选项目

### 魔方生态

从模拟、计时数据迁移到赛事监控——把这项爱好完整地写成了工具链。

| 项目 | 做了什么 |
| :--- | :--- |
| **[cube-simulator](https://github.com/JackPeng-Coder/cube-simulator)**<br>`Python` `Pygame` `Kociemba` | 3D 魔方模拟器。鼠标拖拽转层、滚轮换色染色、空格打乱；自动还原接的是自编译的 **Kociemba 二阶段求解算法**（内嵌 C 源码），不是预设步骤表。 |
| **[timer-bridge](https://github.com/JackPeng-Coder/timer-bridge)**<br>`TypeScript` `pnpm` `SQLite` | 魔方计时器数据互转。csTimer / DCTimer / TwistyTimer 三家的成绩和公式可以互相搬，直接读写 JSON、CSV、SQLite。pnpm monorepo：`core` 定义统一中间格式，三个 adapter 各自翻译，加新计时器只要再写一个包。 |
| **[cubing-events-alert](https://github.com/JackPeng-Coder/cubing-events-alert)**<br>`Python` `Tkinter` `BeautifulSoup` | 盯着 cubing.com 上的中国魔方赛事，有新比赛就弹窗。抓取后与本地存档做 diff，只报新增，不重复打扰；可以标记关注的省份并高亮。 |

### 数学与物理模拟

我最花时间的方向：把公式和方程变成可以拖参数、看反应的程序。

| 项目 | 做了什么 |
| :--- | :--- |
| **[fractal-engine](https://github.com/JackPeng-Coder/fractal-engine)**<br>`TypeScript` `WebGL2` `GLSL` | 手写 WebGL2 + GLSL 分形渲染器，迭代在片元着色器里跑，默认 Mandelbrot 集。平移缩放带惯性衰减，滚轮朝光标位置缩放，移动端支持双指捏合。分形通过 `registerFractal()` 插件式注册，加新分形不用动引擎。 |
| **[pmss-pro](https://github.com/STAR-0501/pmss-pro)**<br>`Python` `Pygame` `物理引擎` | 物理教学数字实验平台，**212 次提交**，自研物理引擎：碰撞检测与响应、弹性碰撞速度守恒、弹簧/杆/绳索约束、引力与库仑力，10 步细分积分。从微观粒子一直到天体运动，并集成 AI 助手，可以用自然语言描述并生成物理场景。<br>▸ [使用手册](https://pmss.starbot.top/help/) · [Release](https://github.com/STAR-0501/pmss-pro/releases) |
| **[caffeine-flow](https://github.com/JackPeng-Coder/caffeine-flow)**<br>`Vue 3` `ECharts` `WebRTC` | 用 **Bateman 双指数药代动力学模型**精确模拟任意时刻体内的咖啡因含量，据此安排摄入节奏和睡眠。曲线分过去 12h 实线与未来 12h 预测段。跨设备同步走 **WebRTC DataChannel 点对点，数据不经过服务器**，离线时用扫码配对兜底。<br>▸ [在线使用](https://jackpeng-coder.github.io/caffeine-flow/) |
| **[equation-arena](https://github.com/JackPeng-Coder/equation-arena)**<br>`JavaScript` `Express` `Canvas` | 回合制数学对战游戏：双方放置区块、写方程，按曲线穿过的区块加减分。自写表达式解析器，支持显式/隐式函数、三角/反三角/双曲/对数/指数，配 KaTeX 实时预览。 |

### 竞赛与算法

| 项目 | 做了什么 |
| :--- | :--- |
| **[turing-complete](https://github.com/STAR-0501/turing-complete)**<br>`Python` `Flask` `AI Agent` `Arduino` | 浏览器里的数字逻辑电路模拟器，**162 次提交、约 1.3 万行**。设计上只有 NAND 一个原子门，AND/OR/XOR 都得自己搭出来——搭出等价电路后系统识别并解锁该门。支持模块封装与嵌套、自动仿真，还有一套 AI 智能体框架可以自动搭电路，并能把电路导出成 Arduino 代码烧录。 |
| **[oi-source](https://github.com/JackPeng-Coder/oi-source)**<br>`C++` `Python` | 洛谷题解与竞赛代码库，按 D1–D8 难度分级归档，刷了 10 个月。**224 题完成 197，完成率 87.95%**。文件名前缀编码完成度（`[40]P1037.cpp`），配自写 `stats.py` 扫描汇总。 |
| **[luogu-contest-alert](https://github.com/JackPeng-Coder/luogu-contest-alert)**<br>`Python` `PySide6` | 监控洛谷比赛状态，在「未开始 → 进行中」的瞬间弹出桌面通知，可一键跳转。支持提前 5/15/30/60 分钟提醒；**按比赛触发点动态对齐检查时间**，没有临近触发点就回退轮询。状态持久化到本地 JSON，跨重启不重复提醒。 |

### 工具与效率

都是自己真的遇到了问题，然后顺手写掉的。

| 项目 | 做了什么 |
| :--- | :--- |
| **[tasklist](https://github.com/JackPeng-Coder/tasklist)**<br>`Vue 3` `TypeScript` `Pinia` `PWA` | 纯前端任务清单：事项可递归嵌套（组合状态由子孙递归聚合）、按状态与日期分组、拖拽排序与合并（拖到组合上即合并）、撤销重做，中英双语 + 深浅主题，19 个测试 + CI。不登录不联网，数据只存在浏览器本地。<br>▸ [在线使用](https://jackpeng-coder.github.io/tasklist/) |
| **[class-desktop-organizer](https://github.com/JackPeng-Coder/class-desktop-organizer)**<br>`Python` `OpenAI API` | 用 AI 把班级电脑桌面上散落的文件按学科自动归位，覆盖 txt/docx/pdf/xlsx/pptx 等格式。带只扫不动的 `--dry-run` 试运行模式，11 个测试，可 pip 安装。 |
| **[end-poem](https://github.com/JackPeng-Coder/end-poem)**<br>`HTML` `CSS` | 《我的世界》终末之诗的网页复刻：Minecraftia 像素字体、星空背景与视差滚动、原版彩色文本，中英双语三个版本。纯 HTML/CSS 单文件，零依赖。 |

> `pmss-pro` 与 `turing-complete` 发布在另一个账号 [@STAR-0501](https://github.com/STAR-0501) 下。

## 数据面板

<div align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=JackPeng-Coder&show_icons=true&hide_border=true&bg_color=0A0C10&title_color=3E63DD&text_color=B8C2CF&icon_color=F2D024&border_radius=10&rank_icon=github" alt="GitHub 统计">
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=JackPeng-Coder&layout=compact&langs_count=8&hide_border=true&bg_color=0A0C10&title_color=3E63DD&text_color=B8C2CF&border_radius=10" alt="语言分布">
</div>

<div align="center">
  <img src="https://streak-stats.demolab.com/?user=JackPeng-Coder&hide_border=true&background=0A0C10&ring=3E63DD&fire=F5A524&currStreakNum=E6EAF0&sideNums=E6EAF0&currStreakLabel=B8C2CF&sideLabels=B8C2CF&dates=6B7684&border_radius=10" alt="连续贡献">
</div>

## 贡献图

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/JackPeng-Coder/JackPeng-Coder/output/snake-dark.svg">
    <img src="https://raw.githubusercontent.com/JackPeng-Coder/JackPeng-Coder/output/snake-light.svg" alt="贡献图贪吃蛇">
  </picture>
</div>

> 这条蛇由本仓库的 [`.github/workflows/snake.yml`](.github/workflows/snake.yml) 每天自动生成到 `output` 分支，不是从别处扒来的静态图片。

## 联系

- **Email** — [jackpeng-coder@qq.com](mailto:jackpeng-coder@qq.com)
- **GitHub** — [@JackPeng-Coder](https://github.com/JackPeng-Coder)
