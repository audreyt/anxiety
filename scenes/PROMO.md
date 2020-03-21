# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[開始遊戲！](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: 所以在我們開始之前， *你* 有什麼閱讀偏好？

`publish("show_options_bottom")`

# intro-start-2

n3: 好，讓我們的故事開始吧...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: 這是一個人類

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: 而這是人類的焦慮

n: _你_ 扮演焦慮

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: 不。不，沒有，沒在聽。我得看下手機。

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: 你的任務是從 *危險* 中保護人類

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: 天啊！你又在把人生和推特一起刷走了！

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: 是啊我在想為什麼我不多坐著然後聽我的內心發言。

`hong({eyes:"neutral"});`

n: 快， 警告他們面臨的 *危險！*

```
bb({eyes:"look"});
```

[哦不，看那個恐怖的新聞！](#act1d_news)

[哦不，那條推文是不是在偷偷說*我們*？](#act1d_subtweet)

[嘿，一張貓喝牛奶的動畫。](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: 哈是啊很可愛，我--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: **貓消化不了牛奶我們竟然在享受對動物的虐待我們真是大爛人**

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```
