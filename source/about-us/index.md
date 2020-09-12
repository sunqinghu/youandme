---
title: 关于我们
date: 2018-12-12 22:14:36
keywords: 关于我们 ● ABOUT US
description: 
comments: false
photos: https://cdn.jsdelivr.net/gh/TRHX/CDN-for-love109.cn@2.1.3/images/about/cover.webp
---
{% raw %}
<div class="moe-mashiro" style="text-align:center; font-size: 30px; margin-bottom: 20px;">[关于LOVE109❤️纪实小屋]</div>
<div id="hello-mashiro" class="popcontainer" style="min-height: 300px; padding: 2px 6px 4px; background-color: rgba(242, 242, 242, 0.5); border-radius: 10px;">
  <center>
  <p>
  </p>
  <h4>
  正在与&nbsp;<ruby>
  LOVE109❤️纪实小屋管家&nbsp;<rp>
  （</rp>
  <rt>
  欢迎来到我们的小屋 mua~😘</rt>
  <rp>
  ）</rp>
  </ruby>
  对话中...</h4>
  <p>
  </p>
  </center>
  <bot-ui></botui>
</div>
<script src="https://cdn.jsdelivr.net/vue/latest/vue.min.js"></script>
<script src="https://unpkg.com/botui/build/botui.min.js"></script>
<script>
function bot_ui_ini() {
    var botui = new BotUI("hello-mashiro");
    botui.message.add({
        delay: 800,
        content: "来啦老弟？我是小屋的管家，等你好久了~👋"
    }).then(function () {
        botui.message.add({
            delay: 1100,
            content: "这里是LOVE109❤️纪实小屋"
        }).then(function () {
            botui.message.add({
                delay: 1100,
                content: "一个记录爱情、记录生活、充满温馨的小屋~"
            }).then(function () {
                botui.action.button({
                    delay: 1600,
                    action: [{
                        text: "然后呢？ 😃",
                        value: "sure"
                    }, {
                        text: "少废话！ 🙄",
                        value: "skip"
                    }]
                }).then(function (a) {
                    "sure" == a.value && sure();
                    "skip" == a.value && end()
                })
            })
        })
    });
    var sure = function () {
            botui.message.add({
                delay: 600,
                content: "😘"
            }).then(function () {
                secondpart()
            })
        },
        end = function () {
            botui.message.add({
                delay: 600,
                content: "![...](https://view.moezx.cc/images/2018/05/06/a1c4cd0452528b572af37952489372b6.md.jpg)"
            })
        },
        secondpart = function () {
            botui.message.add({
                delay: 1500,
                content: "本小屋建立于 2019-1-17 20:00"
            }).then(function () {
                botui.message.add({
                    delay: 1500,
                    content: "两人在2016年10月9日走到了一起❤️"
                }).then(function () {
                    botui.message.add({
                        delay: 1200,
                        content: "男主人专业是软件工程，女主人专业是应用统计"
                    }).then(function () {
                        botui.message.add({
                            delay: 1500,
                            content: "男主人酷爱单车运动，IT男，喜欢倒腾新鲜事物"
                        }).then(function () {
                            botui.message.add({
                                delay: 1500,
                                content: "女主人善良可爱，思维敏捷，将来的数学界她肯定是大哥大"
                            }).then(function () {
                                botui.message.add({
                                    delay: 1800,
                                    content: "他们彼此恩爱，虽然偶尔吵吵闹闹，但都相信彼此是陪伴自己余生的人"
                                }).then(function () {
                                    botui.action.button({
                                        delay: 1100,
                                        action: [{
                                            text: "网站为什么叫“纪实小屋”呢？ 🤔",
                                            value: "why-mashiro"
                                        }]
                                    }).then(function (a) {
                                        thirdpart()
                                    })
                                })
                            })
                        })
                    })
                })
            })
        },
        thirdpart = function () {
            botui.message.add({
                delay: 1E3,
                content: "主人们希望通过文字的形式记录我们的爱情，记录我们的生活，所以叫纪实小屋"
            }).then(function () {
                botui.action.button({
                    delay: 1500,
                    action: [{
                       text: "域名有什么含义吗？ 🤔",
                        value: "why-cat"
                    }]
                }).then(function (a) {
                    fourthpart()
                })
            })
        },
        fourthpart = function () {
            botui.message.add({
                delay: 1E3,
                content: "域名对于主人们来说有着重要的含义"
            }).then(function () {
                botui.message.add({
                    delay: 1100,
                    content: "10月9日是两位主人在一起的日子，他们希望能够一起共度余生❤️"
                }).then(function () {
                    botui.action.button({
                        delay: 1500,
                        action: [{
                            text: "原来如此",
                            value: "why-domain"
                        }]
                    }).then(function (a) {
                        fifthpart()
                    })
                })
            })
        },
        fifthpart = function () {
            botui.message.add({
                delay: 1E3,
                content: "愿天下有情人终成眷属，如果你也有另一半，祝愿你们长长久久❤️，如果还没有，那就要加油咯！"
            }).then(function () {
                botui.message.add({
                    delay: 1600,
                    content: "那么，请尽情参观LOVE109❤️纪实小屋吧！ ^_^"
                })
            })
        } 
}
bot_ui_ini()
</script>
{% endraw %}
---