# act4

```
SceneSetup.act4();
publish("SAVE_GAME", ["act4"]);
Game.FORCE_CANT_SKIP = true;
```

(...5001)

```
publish("set_how_many_prompts", [1]);
Game.FORCE_CANT_SKIP = false;
Game.CLICK_TO_ADVANCE = true;
```

n3: （遊戲已自動儲存）

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
var hong_frame = _.INJURED ? 9 : 0;
publish("act4", ["hong_walks_in",hong_frame]);
sfx("grass_step1", {volume:0.1});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.2});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.25});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.3});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...1667)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...1333)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.20});
```

(...167)

```
publish("act4_hong_sits");
```

(...66)

```
publish("act4", ["hong_transition", "next"]);
sfx("squeak");
```

(...133)

`publish("act4", ["hong_transition", "next"]);`

(...1333)

```
publish("act4", ["hong_transition", "next"]);
sfx("rustle");
```

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1001)

```
publish("act4", ["hong_transition", "next"]);
```

(...333)

```
publish("act4", ["hong_transition", 9]);
sfx("sandwich");
```

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1466)

`publish("act4-out-1");`

(...201)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

```
publish("act4-show-chars");
Game.FORCE_CANT_SKIP = false;
```

(...901)

`hong({body:"sigh_1"})`

(...601)

```
hong({body:"sigh_2"});
bb({eyes:"look_down"});
```

h: *（嘆氣）*

```
hong({body:"hold", eyes:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: 所以這一切到底^他狼的^意義在哪？

`hong({body:"one_up", eyes:"annoyed"})`

h: 我們*能學到*什麼？我*在*耍笨，我的「朋友們」*在*利用我，而且我們差點^他狼的^*死掉了*。

`hong({body:"normal", eyes:"normal"})`

{{if _.INJURED}}
[是啊，更不用說那些醫療費。](#act4a_bill)
{{/if}}

{{if !_.INJURED}}
[是啊，更不用說遭殃的肝。](#act4a_liver)
{{/if}}

[是啊，*確實*是最糟的情況。](#act4a_worst)

[是啊，我是對的。](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: 嗯。還好有全民健保。

`hong({eyes:"annoyed", mouth:"normal"});`

b: 但是儘管如此...我們活下來了！

`hong({eyes:"normal"});`

h: ？

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: 我們肯定把自己的預期壽命砍掉了好幾年...

`bb({eyes:"surprise"});`

b: 但至少我們*還有*預期壽命！我們活下來了！

```
hong({eyes:"surprise"});
bb({eyes:"normal"});
```

h: ？

(#act4b)

# act4a_worst

`bb({eyes:"normal_d"});`

b: 但是儘管如此...

h: 嗯？

`bb({eyes:"surprise"});`

b: 我們活下來了！

(#act4b)

# act4a_right

`bb({eyes:"normal_d"});`

b: 但是...你也是對的。

`hong({eyes:"surprise"});`

h: 嗯？

`bb({eyes:"normal"});`

b: 我*確實*是叫狼來了的那隻狼。所以當*真正的*危險來臨的時候，你-理所當然地-沒有相信我。

`bb({eyes:"surprise_r"});`

b: 但是儘管如此，我們活下來了！

(#act4b)

# act4b

```
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

b: 儘管發生了這所有的一切，我們仍然在這裡。

`hong({eyes:"suspect"});`

{{if _.INJURED}}
h:  我們才剛和死亡擦肩而過，但你看上去還蠻冷靜的嘛。
{{/if}}

{{if !_.INJURED}}
h: 我們才剛和死亡擦肩而過*還轉身打了個招呼*，但你看上去還蠻冷靜的嘛。
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: 這個嘛，和剛才的情況比起來一切都沒那麼可怕了。這也讓我開始思考。

`bb({eyes:"normal", mouth:"normal"});`

b: 也許我對抗你很糟糕，因為這並沒有保護到你...

h: 但是我對抗你*也*很糟糕，因為那隻讓你叫嚷得更嗨...

`bb({eyes:"normal_r"})`

b: 那麼也許...

`bb({eyes:"normal"})`

h: 也許我們沒必要彼此對抗。

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
```

(...301)

`publish("smash",[0]);`

(...2001)

```
publish("smash",[1]);
sfx("smash_glass");
```

(...2601)

```
publish("smash",[2]);
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

(...2001)

`Game.FORCE_CANT_SKIP = false;`

(#act4b_2)

# act4b_2

```
music('dontfight',{fade:5, volume:0.6});
bb({eyes:"annoyed_d"});
```

b: 我不是大壞狼。但我也不是守衛狼。

`bb({eyes:"sad_d"})`

b: 我是隻遍體鱗傷的流浪狗。

`bb({eyes:"sad"})`

b: 我們經歷了太多不好的事情，受到心理創傷或是被輕視冷漠。這就是為什麼我有時反應過度然後：

```
sfx("yaps", {volume:0.6});
bb({body:"yap_1"});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 215;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: 啊啊啊啊啊啊啊啊啊啊啊啊

(...1884)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_CANT_SKIP = false;
bb({body:"normal", mouth:"scream", eyes:"scream_sad"});
```

b: 但是我不*想*當一隻懦弱的狗！我想保護你！我想做一隻好狗狗！

`bb({eyes:"sad", mouth:"normal"});`

b: 人類...你能幫忙馴服這隻狼嗎？

`hong({eyes:"sad"})`

h: 我...我會試試。

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: 好。與情緒建立健康的關係。這需要溝通。所以我們聊聊吧。

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: 接下來的五分鐘會聽上去很矯情，但我們還是要裝出樣子直到達成目的。

```
hong({body:"hands_2", mouth:"normal"});
```

h: 親愛的內心的狼...*你*現在感覺怎麼樣？

n2: 總共使用的恐懼：

n2: *受傷* {{_.attack_harm_total}}, *不被愛* {{_.attack_alone_total}}, *壞人* {{_.attack_bad_total}}

n2: 你想先談哪個恐懼？（其他的可以等會再談）

```
_.a4_fears_discussed = 0;
_.num_thanks = 0;
hong({body:"normal"});
bb({eyes:"normal"});
```

[我害怕我們會受傷。](#act4_harm)

[我害怕我們會獨自一人。](#act4_alone)

[我害怕我們是壞人。](#act4_bad)

# act4_harm

```
_.a4_talked_about_harm = true;
_.a4_fears_discussed += 1;
```

`bb({eyes:"normal_d"})`

b: 我想保護你不受身體上的傷害，

`bb({eyes:"sad_d"})`

b: 但是*整個世界*都看上去很危險。充斥著悲劇和邪惡。

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: 我不知道，由*我*決定的說的話夠多了。*你*怎麼認為，人類？
{{/if}}

{{if _.a4_fears_discussed==2}}
b: 那麼，還是回到你，人類。你怎麼認為？
{{/if}}

{{if _.a4_fears_discussed==3}}
b: 還有別的想法嗎，人類？
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[你是對的。那麼讓我們保護自己吧。](#act4_harm_skills)

[讓我們暴露給*更多*危險吧。](#act4_harm_exposure)

[謝謝。](#act4_thanks) `_.thanks_for = "人身安全";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: 但是...怎麼做？我有尖牙也有利爪，但我只是個隱喻而已。

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: 我們可以學習防身術？加入一個互相保護對方的團體？提高我們的身體素質和社會距離？

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: 也許吧，但是...

[我們從哪開始？](#act4_harm_skills_start)

[如果這些都不奏效怎麼辦？](#act4_harm_skills_work)

[要是我們過於看重了「安全」怎麼辦？](#act4_harm_skills_overboard)

# act4_harm_skills_start

`bb({ eyes:"sad_d" })`

b: 有那麼多需要做的事情，那麼多我們需要修好自己的地方。我們要從哪*開始*？

`hong({ body:"shrug", eyes:"surprise" })`

h: 從現在開始。

`bb({ eyes:"normal", mouth:"narrow" })`

b: 啊？

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: 我們現在就在進行有效溝通，這就會減少錯誤的絕對性，幫助我們更好地察覺危險，

`hong({ eyes:"surprise" });`

h: *這樣*就會保護我們不受傷害！

`hong({ eyes:"normal", mouth:"normal" });`

h: 所以：這*就是*防身術訓練。

`bb({ eyes:"normal_r" })`

b: 蛤。我本來還在期待更多這樣的：

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
hong({ eyes:"sad", mouth:"smile" });
bb({ body:"karate_1" });
sfx("hiya");
```

(...1001)

`Game.FORCE_CANT_SKIP = false;`

(#act4_something_else)

# act4_harm_skills_work

`bb({ eyes:"normal" });`

h: 確實，沒有百分之百能保護我們的方法...

`hong({ body:"one_up" });`

h: 但即使會有百分之一的進步也值得這麼做，對吧？

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: 即使杯子百分之九十九都是空的，你也說它還有百分之一的水？

`bb({ eyes:"normal" });`

h: 如果你正被困在沙漠裡的話，它仍是有價值的。

`bb({ eyes:"closed" });`

b: 好吧。那乾杯吧。

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: 我是說，你無視我的警告就是因為*我*過於看重安全！

`bb({ body:"normal", eyes:"normal" })`

h: 算啦，你是對的。我們會適度地注意安全。做所有事都適度。

`bb({ eyes:"suspect" })`

b: 你說什麼，*所有事*？

`hong({ eyes:"annoyed" })`

h: 適度地做*適度的事*。

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: 感謝你讓你的說辭前後邏輯連貫。

(#act4_something_else)


# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: ***什麼***

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: 我是說，比如有一隻害怕雷聲的狗。

`hong({ body:"hands_1" });`

h: 一種老練訓練員的做法是播放低音量的雷聲，狗冷靜下來了就給它獎勵。

`hong({ body:"hands_2" });`

h: 訓練員在接下來的幾天裡慢慢調高雷聲的音量，直到那條狗完全克服對雷聲的恐懼。

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: 這叫暴露療法！

`hong({ body:"point", eyes:"normal" });`

h: 既然你是狗，這種療法對你應該也有效，對吧？所有哺乳動物都有同樣的急性緊迫反應。

`hong({ body:"normal" });`

[要是我們麻木*過頭*怎麼辦？](#act4_harm_exposure_overboard)

[要是我們遇見的是*真正的*危險怎麼辦？](#act4_harm_exposure_hurt)

[我是狼，不是狗。](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: 那我就溫柔耐心地對待你，直到你被訓成一隻可愛的小狗。

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: 嗷。

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: 我們*才剛剛*看到了要是你失去恐懼會怎樣- 你把自己置於了*真正的*危險境地。

`bb({ eyes:"angry_r", body:"one_up" })`

b: 再說，*過於*麻木不會讓我們變成心理變態嗎？

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: 不久我們就會發現自己在邊吃爆米花邊看鼻菸謀殺毛片！

`hong({ eyes:"annoyed" })`

h: 我...覺得那和雷聲還是有區別的。

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: 但是區別的界線*在哪*，人類？*在哪？！*

`hong({ eyes:"surprise", body:"one_up" })`

h: 我不知道。但*你*可以幫助我！

`hong({ eyes:"normal", body:"normal" })`

h: 和你一起探討協商，我們會畫出那條界線的。

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: 好吧，但我沒有大拇指，所以畫畫那部分得你來做。

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.INJURED}}
b: 比如：我們從^他狼的^*屋頂*跳下去！
{{/if}}

{{if !_.INJURED}}
b: 比如：我們差點從^他狼的^*屋頂*跳下去！
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: 不你是對的，是*有可能*做過頭。

`hong({ eyes:"normal" });`

h: 但那也是為什麼，如果我們使用暴露療法，我們會一小步一小步地向上走。

h: 在發生*真正的*危險之前，我們就停下。

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: 嗯我覺得聽雷聲和戴著高尖帽杵在暴風雨裡還是有區別的。

(#act4_something_else)

# act4_thanks

`_.num_thanks += 1`

{{if _.num_thanks==1}}
(#act4_thanks_1)
{{/if}}

{{if _.num_thanks==2}}
(#act4_thanks_2)
{{/if}}

{{if _.num_thanks==3}}
(#act4_thanks_3)
{{/if}}

# act4_thanks_1

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"annoyed" })`

b: 等等，你沒有其它想對我說的嗎？就只是...「謝謝」？

`hong({ eyes:"surprise", body:"shrug" })`

h: 對呀！謝謝你關心我的{{_.thanks_for}}.

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: 你還好嗎？

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: 你從沒對我說過*謝謝*。

`hong({ mouth:"smile" });`

h: 哦你這個毛茸茸軟綿綿的大可憐狼。

(#act4_something_else)

# act4_thanks_2

h: 即使你反應過度，我依舊感謝你關心我的{{_.thanks_for}}.

`bb({ eyes:"annoyed" })`

b: 等等...你不會是在用「謝謝」來回避對恐懼的討論吧？

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: 唔，事情很複雜。而且我並不總是能準備好答案的。

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: 生活又不會給你提供備好的答案清單。

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: 但現在，我至少可以說聲謝謝。

b: 那麼，也謝謝你，這麼耐心地聽我說。

`bb({ eyes:"closed" });`

b: 你這個沒毛的小動物。

(#act4_something_else)

# act4_thanks_3

h: 雖然你的亂叫嚇到了我，但其實你只是想保護我的{{_.thanks_for}}.

`bb({ eyes:"smile_r" });`

b: 行了行了，你再這樣奉承我，網友們會對我們有什麼奇奇怪怪的想法的。

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h: 得了吧，我只是個脆弱的大學生而你是個巨大的可怕的狼。能發生什--

`hong({ eyes:"normal", body:"point" });`

h: 那什麼，你別回答。

(#act4_something_else)




# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: 我想確保滿足你內心深處對歸屬感的需求...

`bb({ eyes:"sad_u" });`

b: 但是我擔心要是有任何人瞭解了我們- *真實的*我們- 我們會把他們都嚇跑。

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: 我不知道，由*我*決定的說的話夠多了。*你*怎麼認為，人類？
{{/if}}

{{if _.a4_fears_discussed==2}}
b: 那麼，還是回到你，人類。你怎麼認為？
{{/if}}

{{if _.a4_fears_discussed==3}}
b: 還有別的想法嗎，人類？
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[我同意：讓我們努力提升自己的社交生活吧。](#act4_alone_skills)

[我覺得人們是喜歡我們的。一起找找看？](#act4_alone_experiment)

[謝謝。](#act4_thanks) `_.thanks_for = "社會歸屬感";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: 我們可以練習技巧，像是提問，傾聽，強調，開放思想，諸如此類？

`hong({ eyes:"normal_l" });`

h: 或者養成更好的社交習慣，像是安排時間陪朋友，或是固定每隔一段時間就去參加聚會？

`hong({ body:"one_up" });`

h: 還能讓我們適應被拒絕。

`hong({ eyes:"normal" });`

h: 或是分辨出*沒有*在拒絕我們的人，這些人只是累了或是天生長著一張臭臉。

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: 看來選擇有很多。但是關於這個「學習社交技巧」...

[那不會是*擺佈別人*嗎？](#act4_alone_skills_manipulative)

[那不會讓我們*更容易被擺佈*嗎？](#act4_alone_skills_manipulated)

[如果我們還是失敗了呢？](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: 連環殺手不就是特別擅長使用「同理心」讀取受害者的情緒的人嗎？

`bb({ eyes:"annoyed" });`

b: 查爾斯·曼森不就獲得了朋友和追隨者嗎？

`hong({ eyes:"annoyed", body:"chin" });`

h: 嗯，你是對的。

h: 如果我們不是真心實意地*在乎*他人，「社交技巧」將沒有任何意義。

`hong({ body:"normal" });`

h: 總的來說就是，別當個^混球^。

`bb({ eyes:"annoyed", mouth:"smile" });`

b: 真是個激勵人心的宣傳標語。

`hong({ body:"shrug", mouth:"narrow" });`

h: 「別當個^混球^™」

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: 我們會成為門口的擦鞋墊，一邊說著請和謝謝一邊讓人們踩在我們臉上反覆摩擦！

`bb({ mouth:"scream", eyes:"scream" })`

b: 我們要用熱臉貼多少冷屁股，我們的嘴會變得像是塗了棕色的口紅！

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h: 嗯，你是對的。「社交技巧」不能只是取悅他人，也得包括設定*界限*。

`hong( body:"one_up" });`

h: 如果我們的房子沒有牆作為支撐，我們就不能邀請別人進我們家。

```
hong( eyes:"angry", mouth:"narrow" });
bb( eyes:"annoyed", mouth:"smile" });
```

h: 還有...那個口紅的畫面...*嘔？？*

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: 我們可能會失敗。不對，我們*會*失敗的。

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: 而那也沒關係！每個人在剛開始學新東西時都會失敗的！

`hong({ body:"normal", eyes:"normal" });`

h: 所以讓我們一起在失敗中前進吧，好嗎？

`bb({ eyes:"normal_r" });`

b: 當然了，我猜...最壞的情況，我們可以直接跑路，然後整個新身份。

`bb({ eyes:"normal" });`

h: 是啊我覺得在這個年代做到這些只需要花兩個比特幣。

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: 我們可以做些實驗！

`hong({ body:"chin" });`

h: 我們可以約朋友出去玩，重新聯絡以前的朋友，或者就只是和咖啡師閒聊。

`hong({ body:"normal" });`

h: 我覺得我們也許會發現我們比自己想的要更討人喜歡。

`bb({ eyes:"annoyed" });`

[如果這些只是渺小的，廉價的「勝利」呢？](#act4_alone_experiment_cheap)

[如果這給別人造成了負擔呢？](#act4_alone_experiment_burden)

[但只是閒聊無法代表*真實的*我們！](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: 如果我們掛著假笑，我們就不可能和任何人建立真正的聯絡，

`bb({ eyes:"super_sad" });`

b: *但是*如果我們敞開心扉，其他人就會看到我們一團糟的內心！

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: 翻個身。

b: 什麼。

`hong({body:"hands_1"})`

h: 當狗想展示愛和信任的時候，它們會露出肚子使自己變得脆弱。

`hong({body:"one_up"})`

h: 也許我們*還*無法安心變得太脆弱，但只要多練習，

`hong({body:"normal", eyes:"surprise"})`

h: 有一天我們會能夠向人們展示真實的自己- 遭到透頂，但是有人情味。

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: 你獎勵我的話我就翻身。

`bb({ eyes:"normal", mouth:"normal" });`

h: 免了。

(#act4_something_else)


# act4_alone_experiment_cheap

b: 跟咖啡師說聲「嗨」可不是個在交際花奧運會裡能拿金牌的表現。

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: 這是為了*我們*！

`hong({ body:"one_up", eyes:"annoyed" });`

h: 在社交舞臺上，我們的級別連輕如鴻毛都算不上，我們大概...要以夸克為計量單位。

`hong({ body:"normal", eyes:"normal" });`

h: 如果我們非得從渺小的，廉價的「勝利」開始，那就這麼做。在走到第一千步之前得先邁出第一步。

b: 對！也許說了「嗨」之後，我們下一步可以說...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *「你好嗎？」*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *「就那樣吧！」*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: 也許那個咖啡師只想煮點咖啡，而不是被當做測試我們的社交技巧有多菜的*小白鼠*。

`bb({ eyes:"annoyed" })`

h: 這個，如果我們*真成了*人家的負擔...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: 能知道這點也很好！

`hong({ eyes:"normal" });`

h: 我們就可以學習如何主動地詢問另對方感覺舒服的表達方式，瞭解並尊重他人的界限。

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: 你知道的，那些心理諮商小冊子裡寫的關於「人際溝通能力」的玩意兒。

(#act4_something_else)



# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: 我想守護你的道德需求，讓你成為一個更好的人，

`bb({ eyes:"sad_d" })`

b: 但是怎麼感覺在內心深處，我們破碎得...那麼徹底。

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: 而且別跟我說我們*不是*一團糟。我們剛才從*房頂*上跳下去了。
{{/if}}

{{if !_.INJURED}}
b: 而且別跟我說我們*不是*一團糟。我們剛才差點從*房頂*上跳下去了。
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: 我不知道，由*我*決定的說的話夠多了。*你*怎麼認為，人類？
{{/if}}

{{if _.a4_fears_discussed==2}}
b: 那麼，還是回到你，人類。你怎麼認為？
{{/if}}

{{if _.a4_fears_discussed==3}}
b: 還有別的想法嗎，人類？
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[所以我們破碎得徹底。那我們把自己修好吧。](#act4_bad_fix)

[所以我們破碎得徹底。那我們就接受這點吧。](#act4_bad_accept)

[謝謝。](#act4_thanks) `_.thanks_for = "道德幸福感";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: 我們可以慢慢養成更好的習慣，讓我們的人生邁向正軌，獲得價值，

`hong({body:"one_up"});`

h: 如果需要，我們可以尋求專業的幫助-臨床心理師或是諮商心理師。

`hong({body:"normal"});`

h: 總會有辦法修好我們的。

[如果我們沒法完全修好呢？](#act4_bad_fix_cant)

[如果我們修得*太好*了呢？](#act4_bad_fix_too_much)

[我們負擔不起專業幫助。](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: 嘖，我想你是對的。

h: 我們不可能完全修好。

`bb({mouth:"scream", eyes:"scream_sad"});`

b: 啊啊我就知道我們永遠都會是壞掉的！

`hong({eyes:"surprise"});`

h: 但至少我們可以*不那麼*破碎。

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: 傷口會隨著時間癒合，但它們從不消失。而那也沒關係。

`bb({eyes:"annoyed_r"});`

b: 我猜吧。再說，

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: 過去的傷疤*很性感*。

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: 求你別來這套。

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: 我很不想承認，但是...我內心的一部分*想要*繼續保持這份混亂。

`bb({ eyes:"angry" })`

b: 我是說，沒了它，我們不是會成為*無聊的人*嗎？

`bb({ eyes:"sad_r", body:"one_up" })`

b: 沒了它，我們的作品不會變得又陳腐又乏味嗎？

`bb({ eyes:"sad_u", body:"two_up" })`

b: 沒了它，我們還怎麼和同樣有這種混亂的朋友交流？

`bb({ eyes:"sad", body:"chest" })`

b: 如果我們開始對自己的生活感到滿足，我們豈不是會停止驅動自己去幹更偉大的事嗎？

`hong({ MOUTH_LOCK:true })`

h: ...

h: 要是我們甚至對「克服恐懼」...感到恐懼...

h: 我想我們永遠都無法克服恐懼。

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: 哦，對哦！咻！真是令人鬆了一口氣！

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: 「醫生，我很焦慮因為我正花一小時一百的諮詢費來聽你重複*這讓你有什麼感覺？*」

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: 「嗯-嗯。那麼這讓你有什麼感覺？」

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: 嗯，這是很合理的擔憂。

`hong({ eyes:"annoyed", mouth:"sad" });`

h: 很多人都負擔不起心理醫療這件事遭到透頂。

`hong({ eyes:"normal", mouth:"normal" });`

h: 但是儘管如此，還是有一些便宜或是免費的選擇的：

`hong({ body:"chin" })`

h: 互助小組，線上治療，針對學生的/非盈利的健康中心...

`hong({ body:"hands_1" })`

h: 養成像是吃藥啊，按時睡覺啊，定期和朋友聊天啊，學習新鮮事物啊這樣的習慣。

`hong({ body:"hands_2" })`

h: 去圖書館借書來尋找有證據支撐的心理療法...

`hong({ body:"one_up" })`

h: 在遊戲的末尾會有一張完整的資源清單！

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: 嘿，*我們這個*第四面牆沒能持續多久啊。

`hong({ body:"point" });`

h: 有些東西比敘事規範更重要。比如心理健康。

(#act4_something_else)


# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: 我的意思是，心理治療師不就是這麼說的嗎？接受你的所有情緒，哪怕是負面情緒？

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: 等等。

[「接受」是說*放棄*？](#act4_bad_accept_give_up)

[「接受」是說*贊成*？](#act4_bad_accept_approve)

[「接受」是說*就從字面上理解*？](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: 難道你覺得馬丁·路德·金會說，「害，我們不能坐公交前面的位子，讓我們*接受*這點吧」？

`bb({ eyes:"angry_r", body:"two_up" });`

b: 為什麼那些雞湯產業會輸出揮舞白旗是什麼*大智慧*的觀念？

`bb({ eyes:"annoyed", body:"normal" });`

h: 我覺得當醫生說「接受」不好的事物的時候是說： 承認它們的存在，並承認它們很難改變，

h: 但並不是說一定要放棄改變。

`bb({ eyes:"suspect" });`

b: 那他們就該說*承認*，而不是*接受*。

`hong({ body:"chin", eyes:"annoyed" });`

h: 哈這麼一想，「接受」這個詞是有點令人費解。

`bb({ eyes:"closed", mouth:"narrow" });`

b: 嗯哼，我*承認*這點。

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: 像是我們壞掉之類的是件好事？好個毛！

`bb({ eyes:"angry_r", body:"one_up" });`

b: 所有那些美化心理疾病的好萊塢編劇都是垃圾！

`bb({ eyes:"angry", body:"two_up" });`

b: 有心理疾病*糟透了*！它剝奪了人們*生活的權利*！我們為什麼要*接受*？！

`bb({ body:"normal" });`

h: 我覺得當醫生說「接受」我們的情緒的時候是說：多些耐心。

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: 就像在流沙中掙扎只會讓你陷得更深，正確的解決方法是耐心地躺平。

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: 與你，與我的恐懼對抗，讓我跳下了樓頂。
{{/if}}

{{if !_.INJURED}}
h: 與你，與我的恐懼對抗，差點讓我跳下了樓頂。
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: 相反，正確的解決方法是做我們現在正在做的事情- 不是互相對抗，而是耐心地和對方相處。

`bb({ eyes:"annoyed" });`

b: 那他們就該*這麼*說而不是用*接受*這種有問題的詞彙。

`hong({ body:"chin", eyes:"annoyed" });`

h: 哈這麼一想，「接受」這個詞是有點爛。

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: 我不接受*接受*這個詞。

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: 但我們已經*知道*了你不能真的在字面上接受我！

`bb({ eyes:"sad_u", body:"two_up" });`

b: 整個*問題*就在於我想幫助你，但是我不會用語言表達！

`bb({ eyes:"sad", body:"normal" });`

h: 我覺得當醫生說「接受」你的情緒的時候是說： 「不要抗爭或無視它們。」

`hong({ eyes:"surprise", body:"one_up" });`

h: 傾聽你所說的話，和你*一起*討論，但不把你說的都當做百分之百的真理。

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: 那他們就該*這麼*說而不是用*接受*這種模糊又費解的詞彙。

`hong({ body:"chin", eyes:"annoyed" });`

h: 我猜他們的語文也很爛。

(#act4_something_else)




# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: 總之，你還想談什麼嗎？
{{/if}}

{{if _.a4_fears_discussed==2}}
h: 所以，你沉重的小心臟上面還壓著什麼嗎？
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[我害怕我們會受傷。](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[我害怕我們會獨自一人。](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[我害怕我們是壞人。](#act4_bad)
{{/if}}

[不，沒別的了。](#act4c_prelude)

# act4_something_else_2

h: 很好，我覺得我們已經討論完我們所有的恐懼了。

b: 嗯，只有三種恐懼。

h: 對，不多不少。

b: 小菜一碟。

(#act4c)

# act4c_prelude

h: 聊得愉快，搭檔。

(#act4c)

# act4c

```
Game.clearText();
music(null,{fade:3});
bb({body:"normal", eyes:"normal", mouth:"normal", MOUTH_LOCK:true},0);
hong({body:"normal", eyes:"normal", mouth:"normal"},0);
```

b: ...

`hong({MOUTH_LOCK:true},0)`

h: ...

`bb({eyes:"annoyed_d"})`

b: 這並不是什麼*遊戲*，你得知道。

`bb({eyes:"angry_d", body:"one_up"})`

b: 要和你的情緒建立健康的關係並不是戳戳螢幕上的按鍵就能做到的。

`bb({eyes:"sad", body:"normal"})`

b: 我們真的*能*合得來嗎？

b: 我們真的*能*合作嗎，像一個團隊那樣？

`hong({eyes:"sad", body:"one_up"})`

h: 這個嘛，

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: 不，不好意思...

```
Game.clearText();
publish("act4-in-2");
music('campus', {volume:0.5, fade:1});
```

(...2101)

(#act4d)

# act4d

`Game.WORDS_HEIGHT_BOTTOM = 221;`

`publish("act4", ["alshire", 0]);`

a: 你介介介意我和你坐在一塊兒吃午餐嗎？

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *這*就是你喜歡的人？他怎麼一個人坐著，看著像連環殺人狂一樣？
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: 問你喜歡的人你能不能和他坐一塊兒？你知道我們聽上去有多*飢渴*嗎？！
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: *這*就是你喜歡的人？我們打擾了人家的平靜！我們真是個累贅！
{{/if}}

`publish("act4", ["alshire", 2]);`

a: 我- 我是說， 如- 如果不行的話沒關係，我只是...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[等等，我是不是在派對上見過你？](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[嗯，當然可以！過來吧。](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[對不起，我現在想花點時間獨處。](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: 噢你當時在那個沙發上！我第一次去的那個派對...

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: 我當時恐慌發作，打了那個人一拳。
{{/if}}

{{if _.a2_ending=="flight"}}
h2: 我當時恐慌發作，哭著逃跑了。
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: 等等人類，我們好像讓人家尷尬了。

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: 啊，我不是故意要讓你難堪的！

`publish("act4", ["hong_to_alshire",4]);`

h2: 只是想起了一副友善的面孔，僅此而已。

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: **啊啊啊啊啊我就知道！他是個危險的推動恐慌情緒的瘋子！**
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: **啊啊啊我們給別人留下的第一印象是「目睹了我的創傷」！他絕對討厭我們！**
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: **啊啊啊啊我們讓別人想起了痛苦的經歷。我們僅僅存在著就會傷害到別人。**
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: 等等人類，他們看上去有點不自在。

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: 啊，當然了不要覺得有壓力！

`publish("act4", ["hong_to_alshire", 4]);`

h2: 我只是說，如果你想的話你可以坐在這裡。

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: **他表現得*過於*友好了！就像是泰德·邦迪，那個連環殺人犯一樣！**
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: **他只是裝作友好！沒有人*真的*想接近我們！**
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: **啊啊啊我們總是讓別人尷尬！我們是地球上的汙點！**
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: 等等人類，我們可能讓人家尷尬了。

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: 啊，我不是想顯得無禮！

`publish("act4", ["hong_to_alshire", 6]);`

h2: 我只是需要一點時間來處理自己的情緒。請不要把它當做出於個人的拒絕。

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: **他在處理什麼噁心扭曲的想法？！這瘋子的心裡裝的都是什麼黑暗的慾望？！**
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: **我們被出於個人地拒絕了！永遠不會有人愛我們！**
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: **我們打擾了他處理情緒！他將會永遠飽受痛苦而這都是我們的錯！**
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: **快走快走快走快走快走快走快走快走快走快走**

```
Game.clearText();
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["alshire", 10]);
sfx("pop");
```

(...1001)

```
publish("act4", ["alshire", 11]);
sfx("alshire_run");
```

(...2601)

```
publish("act4-out-3");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
```

(...1201)

`publish("act4-jumpcut-hong");`

h: 哈。真奇怪。不知道他剛才在想什麼。

`publish("act4", ["hong_closer", 2]);`

h: 不管了，總之，你剛才在說？

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: 呃，我忘了？什麼關於團隊和合作的？

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: 人們說你要和你的情緒「達成和解」，就好像你的情緒是*戰爭罪犯*一樣。

`publish("act4", ["bb_closer", 7]);`

b: 但是我*不*想我們只是達成和解！我想讓我們成為*盟友*！

`publish("act4", ["bb_closer", 3]);`

b: 我想做只優秀的守衛狗。就像飢餓和口渴感會提醒你有生理上的需求那樣，

`publish("act4", ["bb_closer", 8]);`

b: 我想成為你在*心理*需求上的警鈴- 對安全，歸屬感和道德的需求。

`publish("act4", ["bb_closer", 1]);`

b: 但是...我做的很糟糕，所以我需要你來訓練我。

`publish("act4", ["bb_closer", 4]);`

b: 我並不「總是合理的」，但也不是「總是無理的」。 我只是...在儘自己最大的努力了。所以，拜託，

`publish("act4", ["bb_closer", 30]);`

b: 幫我幫助你吧！

`publish("act4", ["bb_closer", 6]);`

b: 雖然，教一條老狗新技巧*會*花些時間。也許是*好幾年*。

`publish("act4", ["bb_closer", 3]);`

b: 有時我會犯老毛病，不經意間又回到以前的習慣。

`publish("act4", ["bb_closer", 2]);`

b: 我會衝著陰影狂吠。我會用語言恐嚇你。我甚至可能會強迫你看到一些...東西的畫面。

`publish("act4", ["bb_closer", 9]);`

b: 對不起！我是隻遍體鱗傷的流浪狗！受傷的狗有時會拉大便在你的床上！

`publish("act4", ["bb_closer", 4]);`

b: 但是如果你對我有耐心... 然後就只是坐著陪陪我...

`publish("act4", ["bb_closer", 8]);`

b: 也許你可以馴服這隻狼。

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[乖狗狗。](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[乖人類。](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

# act4f-pat-hong

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 13]);
```

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...6501)

`publish("act4", ["bb_closer", 15]);`

(...1001)

(#act4f)

# act4f-pat-bb

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 10]);
```

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...6501)

`publish("act4", ["bb_closer", 12]);`

(...1001)

(#act4f)

# act4f

```
Game.FORCE_CANT_SKIP = false;
publish("act4", ["bb_closer", 16]);
publish("act4", ["hong_closer", 5]);
```

{{if _.fifteencigs}}
b: **啊啊啊啊你還在一個人吃十五根菸啊啊啊啊**
{{/if}}

{{if _.parasite}}
b: **啊啊啊啊你還在對社會毫無貢獻地吃東西我們是社會寄生蟲啊啊啊啊**
{{/if}}

{{if _.whitebread}}
b: **啊啊啊啊你還在吃更多的白麵包啊啊啊啊**
{{/if}}

```
publish("act4", ["bb_closer", 18]);
publish("act4", ["hong_closer", 6]);
sfx("yaps", {volume:0.6});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 205;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: **啊啊啊啊啊啊啊啊**

(#credits)
