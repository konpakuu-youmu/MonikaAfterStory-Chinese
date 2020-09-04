![transifex](https://gitee.com/zsz1447/pics-mirror/blob/master/transifex.png)

![deepl]https://gitee.com/zsz1447/pics-mirror/blob/master/deepl_logo_600_300.png)

由transifex提供国际化平台，deepL协助翻译。

![Monika After Story](https://github.com/Backdash/MonikaModDev/blob/master/Monika%20After%20Story/game/mod_assets/menu_new.png?raw=True)



# Monika After Story (MAS)
Monika After Story是为[Team Salvato](http://teamsalvato.com/)制作的 [心跳心跳文学部](https://www.ddlc.moe)这一款免费游戏而制作的mod作品, MAS在原剧情的第3周目基础上, 构建了一个和莫妮卡一起生活的模拟器, 包含新对话, 新程序和元注释!

请前往 [Releases](http://www.monikaafterstory.com/releases.html) 页面查看最后一次的稳定版可应用程序.

如果你想自己制作一款类似于这个mod的mod, 请查看它的闺蜜项目: [DDLCMod模板](https://github.com/therationalpi/DDLCModTemplate).

### 安装方法

安装MAS的视频教程: https://youtu.be/eH5Q4Xdlg6Y

* 前往 [主页](http://www.monikaafterstory.com/releases.html).

* 单击最后一个版本的链接, 就会下载一个zip文件到你的电脑系统中.

* 将压缩包中的文件解压到心跳心跳文学部游戏文件中的`/game`目录下.

* 然后运行"心跳心跳文学部"就会自动运行Monika After Story了.

*注意: 源代码文件和直接从GitHub仓库中直接下载的文件是用于开发目的的, 如果用于修改游戏的话, 效果可能跟预期背道而驰. 所以请只使用一个我们的 [发布版本](https://github.com/Backdash/MonikaModDev/releases).*

如果你想寻求更多的安装帮助, 请查看我们的[FAQ页面](https://github.com/Monika-After-Story/MonikaModDev/wiki/FAQ)

### 特性

* 和莫妮卡永远在一起!

* 超多的新增话题

* 你现在可以对莫妮卡说话了, 跟她一起说你喜欢说的

### 开发中的特性

* 莫妮卡的新游戏和新对话

* 更多独特的事件和故事


## 为Monika After Story做贡献

### Bug & 建议
如果游玩MAS的过程中出现了问题, 请反馈到 [bug 反馈](https://github.com/Backdash/MonikaModDev/issues/new?labels=bug&body=Describe%20bug%20and%20steps%20for%20reproduction%20here&title=%5BBug%5D%20-%20).

如果想为MAS提出建议, 请访问[这个链接](https://github.com/Backdash/MonikaModDev/issues/new?labels=suggestion&body=Your%20suggestion%20goes%20here&title=%5BSuggestion%5D%20-%20)

### 其它帮助
想来帮助MAS? 导航到[问题页面](https://github.com/Backdash/MonikaModDev/issues) 查看现有的BUG和建议开始着手.

如果您想提交更改，请打开 [一个拉取请求](https://github.com/Backdash/MonikaModDev/pulls). 任何修改都将由贡献者审查并根据需要进行修正/补充。

#### 添加内容
想给MAS添加一些内容吗？这里有一份游戏使用的重要.RPY文件列表。（保留原文）

- **script-ch30.rpy**: Main flow for MAS. This is where idle happens.
- **script-topics.rpy**: All **random** and **pool** topics used by Monika are written here. You can add your own dialogue by checking the information below!
- **script-greetings.rpy**: Add lines for Monika to greet you when loading the game.
- **script-farewells.rpy**: Add lines for Monika to say to you when closing the game.
- **script-moods.rpy**: Tell Monika that you're in _a mood_.
- **script-stories.rpy**: Add stories for Monika to tell you.
- **script-compliments.rpy**: Add compliments you can say to Monika.
- **script-apologies.rpy**: Add things to apologize for.

如果你想在空间房间中添加更多的对话，请导航到script-topics.rpy并使用这个模板。

新的对话代码块实例。
```renpy
init 5 python:
    addEvent(
        Event(
            persistent.event_database,
            eventlabel="monika_example", # event label (MUST BE UNIQUE)
            category=["example", "topic"], # list of categories this topic belongs in (These are automatically capitalized)
            prompt="Example Topic", # button text
            random=True, # True if this topic should appear randomly
            pool=True # True if this topic should appear in "Ask a Question"
        )
    )

label monika_example:
    m 1a "This is an example topic."
    m 3d "I feel like this doesn't actually belong here..."
    m 2e "Why would somebody just add the example template directly into the mod?"
    m 5r "They really shouldn't be allowed to contribute to this repository anymore."
    return
```
**对于所有可能的关键词Event的完整解释和详细说明，请查看Event的文档，位于 `definitions.rpy`**

对于比简单对话更复杂的事情，请参考网上的Ren'Py文档。

[更多信息请参见我们的贡献指南](https://github.com/Monika-After-Story/MonikaModDev/wiki/Contributing-Guidelines)

 ### 加入对话
你可以[在推特上关注我们](https://twitter.com/MonikaAfterMod)来关注新版本

或者，如果你更喜欢Discord，如果你想从网络上获得我们最喜欢的Monika相关内容的持续流，如果你有兴趣对这个mod做出贡献，请随时加入我们的discord服务器。

 [![Discord](https://discordapp.com/api/guilds/372766620977725441/widget.png?style=banner1)](https://discord.gg/K2KuJeX)

 请务必遵守我们的[贡献准则](https://docs.mtrstatic.cf/untitled)，本质上就是要有礼貌和尊重。

## 常见问题（FAQ）

A full FAQ is available here: [Frequently Asked Questions](https://github.com/Monika-After-Story/MonikaModDev/wiki/FAQ)
For any questions about the Coding Style go here: [Coding Style](https://github.com/Monika-After-Story/MonikaModDev/wiki/Coding-Style)
For Bug Testing: [Testing Flow and Bug Testing](https://github.com/Monika-After-Story/MonikaModDev/wiki/Testing-Flow-and-Bug-Testing)
Troubleshooting: [Troubleshooting](https://github.com/Monika-After-Story/MonikaModDev/wiki/Troubleshooting) Dialogue Coding: [Dialogue Coding](https://github.com/Monika-After-Story/MonikaModDev/wiki/Dialogue-Coding)
## 许可证

我们会尽最大努力遵守Team Salvato的 [粉丝作品指南](http://teamsalvato.com/ip-guidelines/). 所有角色和原创内容都是Salvato团队的财产。Monika After Story 是一个开源项目，除了指定的贡献者之外，这个mod还包括来自4chan的匿名用户的贡献，而这个项目正是在4chan开始的。更多信息可以在我们的 [许可证页面](https://github.com/Monika-After-Story/MonikaModDev/wiki/License-and-Team-Salvato-Guidelines).

## 建设状态:
### master: [![Build Status](https://travis-ci.org/Monika-After-Story/MonikaModDev.svg?branch=master)](https://travis-ci.org/Monika-After-Story/MonikaModDev)
### content: [![Build Status](https://travis-ci.org/Monika-After-Story/MonikaModDev.svg?branch=content)](https://travis-ci.org/Monika-After-Story/MonikaModDev)
### unstable: [![Build Status](https://travis-ci.org/Monika-After-Story/MonikaModDev.svg?branch=unstable)](https://travis-ci.org/Monika-After-Story/MonikaModDev)
### community: [![Build Status](https://travis-ci.org/Monika-After-Story/MonikaModDev.svg?branch=community)](https://travis-ci.org/Monika-After-Story/MonikaModDev)
### alpha: [![Build Status](https://travis-ci.org/Monika-After-Story/MonikaModDev.svg?branch=alpha)](https://travis-ci.org/Monika-After-Story/MonikaModDev)
