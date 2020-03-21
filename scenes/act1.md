# act1

```
SceneSetup.act1();
```

(...300)

n: 而這是人類的焦慮

n: _你_ 扮演焦慮

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}



# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: 哦嗨！我們又回來了？

`hong({eyes:"0_neutral"})`

n: 你的任務是從 *危險* 中保護人類

`bb({eyes:"look", mouth:"small_lock"})`

n: 實際上，重玩這個遊戲正讓他處於 *危險中*

n: 快，警告他！

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: 人類！ 聽著，我們碰到危險了！ 這個玩家...

[...要再次折磨我們！](#act1_replay_torture)

[...不可能找到別的結局！](#act1_replay_alternate)

[...會發現遊戲的內容和結構相矛盾！](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: 他會讓我們縮成球球然後哭哭！
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: 他會讓你恐慌發作以謀殺你的手機！
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: 他會讓我們*不*揍派對上的那個人！
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: 他會讓我們揍派對上那個混亂善良的人！
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: 呃至少我們這回也許不用從屋頂上跳--
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: **他會讓我們從屋頂上跳下去的。**
{{/if}}

`bb({body:"fear"});`

b: **所有這些新的壞事都會發生在我們身上，然後我們就會--**

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: 當然了，*總體來說*整個故事還是一樣的，但是每章都有兩個可能的結局，再說還有那麼多對話分支的選--

`bb({body:"fear"});`

b: 那個玩家會很失望，關掉這個頁面，刪掉這個程式，然後我們就會--

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: 會發現——什麼呢？

`bb({eyes:"normal"});`

b: 整個故事想闡述的，就是你可以如何***選擇***與你的恐懼建立健康的合作關係，

`bb({eyes:"normal_right"});`

b: 但是重玩遊戲只會看到同一個故事，也就是在暗示你的***選擇***壓根不重要，

`bb({eyes:"narrow_eyebrow"});`

b: 也就是說遊戲想傳達的意義，和遊戲的機制根本就互相矛盾，

`bb({eyes:"fear"});`

b: 於是這個敘事宇宙的結構會開始瓦解，

`bb({body:"fear"});`

b: 然後我們就會--

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: **死掉！！！！！！**

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.clearText();
```

(...1001)

```
bb({body:"laugh"});
hong({body:"laugh"});
Game.clearText();
sfx("laugh");
```

(...5001)

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"0_sammich"});
```

h: 好了回到角色來吧。

```
Game.clearText();
```

n4: （讓 _你的_ 焦慮吧啦吧啦選擇和 _你的_ 恐懼吧啦吧啦你知道怎麼玩的）

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: 哦妙啊，我的狼回來了。太————棒了。

`hong({eyes:"0_neutral"})`

n: 你的任務是從 *危險* 中保護人類

`bb({eyes:"look", mouth:"small_lock"})`

n: 實際上，那個三明治正讓他處於 *危險中*

n: 快，警告他！

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: 人類！聽著，我們碰到危險了！危險是...

`bb({body:"squeeze"})`

n4: （讓 _你自己的_ 焦慮來接手遊戲！ 選擇和 _你的_ 恐懼最接近的選項）

(#act1_normal_choice)

# act1_normal_choice

[我們又在一個人吃午餐！](#act1a_alone) `bb({body:"squeeze_talk"})`

[我們吃東西並不能產生價值！](#act1a_productive) `bb({body:"squeeze_talk"})`

[白麵包對我們有害！](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: 你不知道孤獨和一天抽十五根菸一樣會導致過早死亡嗎？

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: （Holt-Lunstad 2010，醫學期刊)

`hong({eyes:"0_annoyed"})`

h: 呃，感謝你標註來源但是--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: 也就是說如果我們*現在*沒和別人待在一塊兒我們就會-

`bb({body:"panic"})`

b: **死掉！！！！！！**

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: 你使用了 *不被愛的恐懼*

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: 趕快掏出你的電腦幹點正事！

`hong({eyes:"0_annoyed"})`

h: 呃，我不想讓麵包屑掉到鍵--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 如果我們沒有在為社會做貢獻我們就是社會寄生蟲！

b: 就會有社會體系裡的社會醫生用藥來消滅社會寄生蟲然後我們就會--

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: **死掉！！！！！！**

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: 你使用了 *成為壞人的恐懼*

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: 那些研究有沒有做重複實--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 澱粉會導致我們血糖飆升然後我們不得不被截掉四肢然後我們就會-

`bb({body:"panic"})`

b: **死掉！！！！！！**

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: 你使用了 *受到傷害的恐懼*

(#act1b)

# act1b

n: 效果非常顯著

`bb({mouth:"smile", eyes:"smile"});`

b: 看到了嗎，人類？我是你忠誠的守衛狼！

`bb({body:"pride_talk"});`

b: 相信你的直覺！你的感受永遠是合理的！

`bb({body:"pride"});`

n: 讓人類的能量條歸零

n: 為了保護人類生理上、社會上、道德上的需求，你可以使用：

n: *受到傷害的恐懼* #harm#

n: *不被愛的恐懼* #alone#

n: 和 *成為壞人的恐懼* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: （重要提示： 選擇那個說中了你內心最深處最隱祕的恐懼的選項！）

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: 哈我覺得我好像應該看一下手機了。

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: 保護你的人類

n: 抵擋這個世界。 抵擋其他人。 抵擋他自己。

n: 祝你好運

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: 第一輪： *FIGHT!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: 哈。臉書推送說這個週末有場派對。

`bb({eyes:"uncertain"});`

b: 那個怪胎難道不是*每個*週末都辦派對嗎？

`bb({eyes:"uncertain_right"});`

b: 他到底是有多空虛？肯定在內心深處是一團糟！

`hong({eyes:"surprise"});`

h: 還有，我被邀請了？

`bb({eyes:"fear", mouth:"normal"});`

b: 那麼！

[接受，否則我們會孤獨到死掉！](#act1c_loner)

[拒絕，那兒全是嗑藥的！](#act1c_drugs)

[無視，我們只會讓派對變悲傷。](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: 一天十五根菸，人類！十五根！
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: 然後我們的葬禮上會一個人都沒有，他們會把我們的骨灰揚到海里，我們會被鯨魚吃掉，
{{/if}}

{{if !_.fifteencigs}}
b: 然後我們就會成為**鯨魚的大便**！
{{/if}}

{{if !_.fifteencigs}} `_.whalepoop = true` {{/if}}

(...500)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

{{if !_.fifteencigs}}
b: 所以我們當然要去那個派對！
{{/if}}

{{if _.parasite}}
b: 但是要帶上電腦所以我們可以工作，避免當個社會寄生蟲。
{{/if}}

{{if _.whitebread}}
b: 只要他們不提供**白麵包**
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: **老天啊**。 要是那能讓你閉嘴的話，行。

h: 我會同意。

{{if _.whalepoop}}
b: 鯨魚的大便啊，人類！ 鯨魚的大便！
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: 或者更糟... **白麵包**
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: 我們嗑的白麵包會嚴重過量！ 我們腫脹的屍體都塞不進焚化爐！
{{/if}}

{{if !_.whitebread}}
b: 我們會嗑多少藥！ 殯儀館的人都會奇怪這具屍體怎麼已經*提前*防腐過了！
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: 再說，不能參加派對，我們必須工作否則就是糟糕的社會寄生蟲！
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: **老天啊**。 要是那能讓你閉嘴的話，行。

h: 我會拒絕。

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: 我們只會找個角落哭哭自己的孤獨是如何像一天十五根菸一樣致命。
{{/if}}

{{if _.parasite}}
b: 我們在派對上只會一直擔心要怎麼做才能產生價值。
{{/if}}

{{if _.whitebread}}
b: 我們只會一直擔心不健康的食物選擇會讓我們怎麼死掉。
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: 哇哦為什麼呢。

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: 所以要是我們去了我們就會讓他們感覺糟糕，但如果拒絕了邀請我們也會讓他們感覺糟糕！

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: **我們只會讓別人感覺糟糕，所以我們應該感覺糟糕**

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: 呃。要是那能讓你閉嘴的話，行。

h: 我會無視邀請。

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: 總之。臉書雜訊太多了。 我需要更平靜，不那麼容易引發焦慮的東西。

`hong({eyes:"neutral"});`

h: 現在推特上有什麼？

`bb({eyes:"look"});`

[哦不，看那個恐怖的新聞！](#act1d_news)

[哦不，那個推文是不是在偷偷說我們？](#act1d_subtweet)

[嘿，一張貓喝牛奶的動畫。](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: 天啊，感覺像是整個世界都燒起來了，你說是吧？

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: 就好像一切都在邁向結束，所有事物都在消亡。 然而我們命中註定，在劫難逃。

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: 我們把這個新聞轉發吧！

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.badnews=true`

```
music('battle', {volume:0.5});
hong({mouth:"anger", eyes:"anger"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: 好好我會轉發的所以拜託你安靜！

`hong({mouth:"neutral", eyes:"annoyed"});`

h: 去他的，還是看下限時動態吧。

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: 這是條在暗示我們的推文！ 一條卑鄙、狡猾（沒有 @ 當事人的）嘲諷推文！

`hong({eyes:"annoyed"});`

h: 也許不是？

`bb({eyes:"narrow", mouth:"small"});`

b: 但是萬一他們全都在背地裡議論我們呢？

h: 他們沒--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: **正對著我們的背後**

`hong({eyes:"sad", mouth:"sad"});`

h: 我不覺--

`bb({eyes:"narrow", mouth:"small"});`

b: 但是*萬一*

h: 閉--

`bb({eyes:"narrow_eyebrow"});`

b: *萬一*

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
hong({mouth:"shut"});
```

h: ...

(...1000)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.subtweet=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: 好————了，還是看看限時動態吧。

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: 哈是啊很可愛，那就轉發一下吧，我覺--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: **貓消化不了牛奶我們竟然在享受對動物的虐待我們真是大爛人**

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("18p", "bad");
```

(...2500)


`_.catmilk=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: 好————了，還是看一下限時動態吧。

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: 唔，昨晚的照片。所以*這*就是那些週末派對的樣子。

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: 哎喲。好像太多人了。

h: 也許我不該同意那個邀請的？

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[改變我們的決定？像個混蛋那樣？！](#act1e_yes_dontchange)

[改變我們的決定！太多人了！](#act1e_yes_changetono)

{{if _.subtweet}}
[對他們絕對在偷偷議論我們。](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[等等我們還沒查核事實就轉發了。](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[嘿你現在的姿勢很糟糕你知道嗎？](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 他們就等著我們來，結果我們卻背叛他們的信任？你想注孤生嗎？！

{{if _.fifteencigs}}
b: **十五。根菸。**
{{/if}}

{{if _.whalepoop}}
b: **鯨魚。大便。**
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: 閉嘴閉嘴我不改了！

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 你不知道踩踏事件都是怎麼來的嗎？

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 2003年羅德島的一家夜總會發生火災，混亂中所有人都擠在了出口，於是一百個人被燒死了-

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: **你想讓這種事也發生在我們身上嗎**-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: **拒絕拒絕拒絕拒絕拒絕拒絕拒絕拒**-


```
bb({body:"normal", eyes:"fear", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
hong({eyes:"anger", mouth:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: 閉嘴閉嘴我改成拒絕就是了！老天啊！

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: 嗯...看上去真的很有趣。

h: 也許我不該拒絕那個邀請的？

`bb({mouth:"normal", eyes:"normal"});`

[改變我們的決定？像個混蛋那樣？！](#act1e_no_dontchange)

[改變我們的決定！別孤獨地死掉！](#act1e_no_changetoyes)

{{if _.subtweet}}
[對他們絕對在偷偷議論我們。](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[等等我們還沒核查事實就轉發了。](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[嘿你現在的姿勢很糟糕你知道嗎？](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: 每個人都在指望我們！

b: ...讓他們有一個完美的派對，沒有噁心的{{if _.whitebread}}、大嚼特嚼白麵包的{{/if}}討厭鬼，比如你--


```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
bb({body:"normal", eyes:"uncertain", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: 閉嘴閉嘴我不改了！

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 慢性孤獨會導致產生過多的皮質醇，提高心血管疾病和中風的風險！

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: **十五。根菸。**
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: 閉嘴閉嘴我改成同意就是了！老天啊！

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 我們要因為所有有問題的推特遭到惡報了！

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: 我們會被找出來登出賬號然後被綁在馬背上的繩子拖著沿資訊高速公路摩擦！

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: 你為什麼要這樣？！

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 我們正在散播謠言！我們正在濫用言論自由摧毀自己的信譽！

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 我們就是法西斯主義從民主廢墟中誕生的原因！

```
bb({body:"normal", eyes:"anger"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
_.factcheck = true;
```

h: 你為什麼要這樣？！

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 你的脊椎是捲餅做的嗎？！別弓著腰看螢幕了！

```
bb({body:"meta"});
```

b: 沒錯也是在說你。

```
bb({body:"normal", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: 你為什麼要這樣？！

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: 嗯...看上去真的很有趣。

h: 也許我不該無視那個邀請的？

`bb({mouth:"normal", eyes:"normal"});`

[繼續無視，我們仍然是派對粥裡的老鼠屎。](#act1e_ignore_continue)

[不如就同意吧。](#act1e_ignore_changetoyes)

[不如就拒絕吧。](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: 不過一直無視別人有點不禮貌，不是嗎？

`bb({eyes:"normal_right"});`

b: 反正其他人也一直在無視*我們*，所以

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: 所以就算是扯平了吧。

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: 你是在...讓我去玩？

b: 嗯哼，我是說，孤獨真的*會*殺死我們的。

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: 那裡人太多了。人多是很危險的。

(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: 隨便吧。有新的配對提醒。

`bb({eyes:"uncertain"})`

b: 什麼，那個約炮app？

`hong({eyes:"annoyed"})`

h: 它不是約炮app，它只是可以用來認識新朋--

`bb({eyes:"narrow"})`

b: 它就是個約炮app。

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: 噢，我配對成功了！看上去挺可愛的！

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: 求求你不要毀了我這次--

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: **危險危險危險危險危險危險危險危險**

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[我們在*被*別人*利用*。](#act1f_used_by_others)

[我們只是在*利用*別人。](#act1f_using_others)

[**你的配對是個連環殺人狂**](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: 隨機約炮也許可以填補下面的空缺，

b: 但是它們永遠無法填補...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: *這裡*的空缺。

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 重點在於**我們會一個人孤獨到死**

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: 你以為別人的生殖器是等待被收集的寵物小精靈嗎？

```
bb({body:"sing", eyes:"pretty", mouth:"shut"});
music("pokemon");
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

```
Game.FORCE_TEXT_DURATION = 1000;
Game.FORCE_NO_VOICE = true;
```

b: ♫ （寶可夢主題曲）-

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ 我要成為，最^淫蕩^的-

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ 其他人無法企及-

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ 大腿和^屁股^，豐滿的胸部-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ 還有汗津津的^屌屌^和^蛋蛋^！-

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ **寶可夢！得抓住**-

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 重點在於我們是個擺佈別人的混蛋。

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`_.pokemon=true`

(#act1g)

# act1f_killer

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.whitebread}}
b: 他會把你困在井裡逼你吃白麵包發胖然後他就可以像穿大衣一樣穿你的皮！
{{/if}}

{{if _.parasite}}
b: 他會用番茄鐘敲你，一邊說「**你該產生點價值的你這個寄生蟲**」
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: 他會把你的肉撕成血色的碎片，把內臟裁成裝飾帶，然後把你的血混入大酒缽攪拌！
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: 把**那個**作為派對邀請怎麼樣？！
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.serialkiller=true`

(#act1g)

# act1g

```
bb({body:"normal", mouth:"normal", eyes:"look"});
hong({body:"2_tired"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
music(false);
```

h: ...

(...500)

h: 我真受夠這個遊戲了。

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}「孤獨會殺死我們」... {{/if}}
{{if _.parasite}}「我們是社會寄生蟲」... {{/if}}
{{if _.whitebread}}「別吃那個，會致命的」... {{/if}}
{{if _.subtweet}}「他們在背後議論我們」... {{/if}}
{{if _.badnews}}「世界在燃燒」... {{/if}}
{{if _.hookuphole}}「我們會一個人孤獨到死」... {{/if}}
{{if _.serialkiller}}「他是個連環殺人狂」... {{/if}}
{{if _.catmilk}}「貓不能消化牛奶」... {{/if}}
{{if _.pokemon}}一個拙劣的模仿歌曲... {{/if}}

h: 我只想過我自己的生活。

h: 我只想擺脫所有這些...痛苦。

`bb({eyes:"look_sad"});`

b: 嘿...人類...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: 會沒事的。

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: 作為你忠實的守衛狼，我會時刻提防危險，努力保證你的安全。

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: 我保證。

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: 最後一個app，Instagram。上面有什麼？

`hong({eyes:"sad"});`

h: 是...更多的派對照片。

`hong({mouth:"sad"});`

h: 每個人都看起來很快樂。無拘無束。無憂無慮。

`hong({mouth:"anger"});`

h: 老天啊，為什麼我不能像他們一樣？為什麼我不能就做個*正常人*？

`bb({eyes:"normal_right"});`

b: 說到派對，關於這個週末的邀請，這是我的**最終**決定。

`bb({eyes:"normal"});`

[我們應該去。](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[我們不該去。](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: 我們--

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: *^操^*。

`hong({body:"2_you"});`

h: 你。

(...500)

b: 什

(...1500)

`bb({eyes:"wat_2"});`

b: 什麼？

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: 我會**同意**去這場派對，

{{if _.act1g=="go"}}
h: **不是**因為你想讓我去，而是因為**我**想去。
{{/if}}

{{if _.act1g=="dont"}}
h: 正是**因為**你不想讓我去。
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: 你**無法**控制我。

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: 現在，麻煩您^幹你狼的^讓我一個人在平靜中吃這個美味的三明治。

`hong({body:"2_sammich_eat"});`

(...601)

```
sfx("sandwich");
hong({body:"2_sammich_eaten", eyes:"0_lookaway", mouth:"0_chew1"})
```

(...601)

```
bb({body:"normal", eyes:"uncertain", mouth:"shut"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
```

b: ...

```
bb({eyes:"normal_right"});
Game.OVERRIDE_TEXT_SPEED = 1;
```

b: ...

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 4;
```

b: ..................

(...500)

`bb({mouth:"normal"});`

[**啊啊啊啊我們要死了**](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[**啊啊啊啊每個人都討厭我們**](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[**啊啊啊啊我們真糟糕**](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: **啊啊啊啊我們要死了啊啊啊啊啊啊**

```
hong({body:"3_defeated1"});
attack("100p", "harm");
```

(...2500)

(#act1i)

# act1h_loneliness

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: **啊啊啊啊每個人都討厭我們啊啊啊啊啊啊**

```
hong({body:"3_defeated1"});
attack("100p", "alone");
```

(...2500)

(#act1i)

# act1h_worthless

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: **啊啊啊啊我們真是爛人啊啊啊啊啊啊**

```
hong({body:"3_defeated1"});
attack("100p", "bad");
```

(...2500)

(#act1i)

# act1i

```
bb({mouth:"smile_lock", eyes:"smile", body:"normal"});
music('battle', {volume:0.5});
```

n: 恭喜

(...500)

n: 你成功地保護了人類生理上、社會上、道德上的需求

n: 看哪，他多感激！

(...500)

n: 現在人類的能量條歸零了，你可以直接控制他的行為

`bb({mouth:"smile", eyes:"normal"});`

n: 選擇你的最後一擊

`bb({mouth:"small_lock", eyes:"fear"});`

n: *解決他*

[{攻擊：懲罰給你帶來焦慮的手機！}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{逃跑：縮成球然後哭！}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: 你的手機讓你恐慌發作！

`bb({eyes:"anger"})`

b: 祖克柏和他的同夥，正為了風投資金操縱你的心理健康！

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 懲罰你的手機！毀了它！滅了它！

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: **殺了它殺了它殺了它殺了它殺了它殺了它殺了它殺了它殺了它殺了它殺了**--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: 整個世界都充滿了危險！

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 像穿山甲那樣！縮成球來自我防衛！

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: **縮起來哭縮起來哭縮起來哭縮起來哭縮起來哭縮起來哭縮起來哭縮起來**--

(#act1j)

# act1j

`SceneSetup.act1_outro()`
