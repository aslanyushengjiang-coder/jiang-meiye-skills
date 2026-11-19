# jiang-meiye-skills · 美业 Skill 导航

开美容院、美甲店、理发店，想让 AI 帮忙，但不知道有哪些现成的 Skill 能用？这里把 GitHub 上开源的、美业门店用得上的 Skill 收到了一起，按店型和工种分好类，带一个本地网页，也能装进 AI 里直接问。

![美业 Skill 导航首页](examples/home.png)

## 里面有什么

- **1,478 个开源 Skill**，来自 384 个 GitHub 仓库，每个都有中文名和一句话说明。
- **6 类店型**：美容护肤、医美、美甲美睫、美发、彩妆造型、养生 SPA，另有一栏“门店通用”。
- **10 个工种**，照一家店从定位到留客的顺序排：定位人设、内容种草、短视频直播、图片海报、同城拓客、咨询预约、到店成交、复购留客、门店管理、合规避坑。
- **按流程找**：选一类店，把这十步每一步能用的 Skill 列出来。
- **一段话就能装**：点开任何一个 Skill，复制那段写好的话发给你的 AI，它会去把这个 Skill 装上。

这 1,478 个里，专门给美业做的有 59 个，比如美容院预约排期和提醒、医美面诊效果图、照片转美甲款式图、脸型发型和妆造搭配建议。其余是各种门店都能用的：种草笔记、同城短视频脚本、海报、客服话术、顾客回访。专门的排在前面。

Skill 是一份装进 AI 里的工作说明，装上之后 AI 会按固定的方法干一件具体的事。

## 怎么用

### 方式一：打开网页自己挑

在线直接看：<https://aslanyushengjiang-coder.github.io/jiang-meiye-skills/>

打不开的话，下载这个仓库，双击 `assets/meiye-skills.html`，用浏览器打开就行，不用联网，不用账号。

左边选店型，上面选工种，中间搜你要干的活（比如“种草笔记”“探店脚本”“回访”）。点开卡片能看到中文说明、来源仓库、开源许可和安装用的那段话。

### 方式二：装进 AI 里直接问

你的 AI 得是装在电脑上、能自己安装 Skill 的那种。把下面这段话发给它：

```text
帮我安装“美业 Skill 导航”这个技能，下载地址：https://github.com/aslanyushengjiang-coder/jiang-meiye-skills
装好后告诉我“装好了”，再用一句话说它能帮我干什么。
```

装好之后直接说：

> 我开美容院，有没有能帮我做同城短视频的 Skill？
>
> 我刚开了家美甲店，从拓客到留客要装哪些 Skill？
>
> 打开美业 Skill 导航的网页。

会用命令行的也可以自己放：

```bash
git clone https://github.com/aslanyushengjiang-coder/jiang-meiye-skills.git ~/.claude/skills/jiang-meiye-skills
```

其他 AI 工具把文件夹放进它自己的 Skill 目录即可。查找脚本需要 Python 3.8 以上，不用装别的库：

```bash
python3 scripts/find.py --query "同城 短视频" --shop 美容护肤
python3 scripts/find.py --flow 美甲美睫
python3 scripts/find.py --stats
```

## 说明

- 每个 Skill 归原作者所有，许可看各自仓库的 LICENSE。这里只放名称、说明、链接和许可信息，不复制 Skill 正文。
- 哪些 Skill 美业门店用得上，以及每条的中文名、说明、店型和工种，由 AI 按作者写的说明判断和标注，来源见 [NOTICE.md](NOTICE.md)。
- 目录更新于 2026-11-19。

## 致谢

感谢每一位把自己的 Skill 开源出来的作者。发现哪条标错了、漏了哪个仓库，欢迎提 Issue。

做电商的看这里：[jiang-ecom-skills · 电商 Skill 导航](https://github.com/aslanyushengjiang-coder/jiang-ecom-skills)。

## 许可

本仓库自己的代码、页面和目录整理部分用 [MIT License](LICENSE)。收录的各个 Skill 以其原仓库的许可为准。
