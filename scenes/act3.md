# act3

```
SceneSetup.act3();
Game.WORDS_HEIGHT_BOTTOM = 205;
sfx("cheers");
```

r: 乾杯！

```
publish("act3",["roofhunter",1]);
publish("act3",["roofhong",1]);
sfx("drinking");
```

(...4001)

```
publish("act3-alpha", ["dizzyhunter",1]);
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",3]);
```

h2: *啊*這個感覺才對。

```
publish("act3",["roofhunter",2]);
publish("act3",["roofhong",2]);
```

r: 你懂的，孩子...

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",6]);
```

h2: 尤其是...上頭的時候...左右杏仁體那一塊...

```
publish("act3",["roofhunter",8]);
publish("act3",["roofhong",5]);
```

r: 你讓我想起我小時候，也被腦子裡的那個怪獸折磨的時候。

```
publish("act3",["roofhunter",9]);
publish("act3",["roofhong",2]);
```

r: 我很高興可以把經驗傳授給你，然後幫你幹掉那頭野獸，就像我當時做的那樣。

```
publish("act3",["roofhunter",2]);
```

r: 嘿，快問快答：真心話還是大--

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",7]);
publish("act3-alpha", ["dizzyhong",0]);
```

h2: **大冒險！**

```
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",2]);
```

r: 哈哈哈！好！

```
publish("act3",["roofhunter",21]);
publish("act3",["roofhong",4]);
```

r: 那，你看到下面那個淡藍色的泳池了嗎？

```
publish("act3-alpha", ["dizzyhong",0]);
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",9]);
```

h2: 嗯？六層樓下面的那個？

```
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",8]);
```

r: 跳進去。

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",10]);
```

h2: ...

```
publish("act3",["roofhong",11]);
```

h2: 呃？等等？

```
publish("act3",["roofhong",10]);
publish("act3",["roofhunter",2]);
```

r: 腦子裡的怪獸要回來了對不對？

```
publish("act3",["roofhunter",23]);
```

r: *噢不不不那個太危險了千萬別別別*--

```
publish("act3",["roofhunter",22]);
```

r: 但這就是為什麼需要這種極限的刺激！盡情派對！及時行樂！人一輩子就活一次， #YOLO！

```
publish("act3",["roofhunter",10]);
```

r: 讓那個東西知道我們^他狼的^根本就不在乎它的^狼言狼語^！跳進去。

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",13]);
```

h2: 呃，但是有時候，呃...恐懼是有它的理由的...

```
publish("act3",["roofhunter",5]);
publish("act3",["roofhong",12]);
music(null, {fade:2});
```

r: ...

```
publish("act3-alpha", ["dizzyhunter",0]);
publish("act3",["roofhunter",6]);
publish("act3",["dd",1]);
```

r: 有沒有搞錯？你是不是信了那個什麼速成正念說的，*感覺到糟糕是一種好事*的說法？

```
publish("act3",["roofhunter",17]);
```

r: 那些操縱這個世界的^混蛋^給我們其餘人帶來了焦慮和抑鬱，

```
publish("act3",["roofhunter",18]);
```

r: 然後在TED演講上告訴我們要「接受」^該死^的生活，「擁抱」我們腦子裡殘忍的惡魔！

```
publish("act3",["roofhunter",6]);
```

r: 孩子我知道*你*明白那些怪獸就是在*傷害*我們這種人，在*折磨*我們這種人。

```
publish("act3",["roofhunter",19]);
```

r: 那不是我們的朋友，那是野獸，凶猛的野獸，需要被放倒然後關起來的野獸，

```
publish("act3",["roofhunter",20]);
```

r: 或者直接*一槍爆頭*。

```
publish("act3",["roofhunter",27]);
```

r: 不然的話，你會任由它戰勝你的。

```
publish("act3",["roofhunter",31]);
publish("act3",["roofhong",14]);
publish("act3",["dd",2]);
```

h2: 對，說的沒錯。

```
publish("act3",["roofhunter",13]);
publish("act3",["roofhong",15]);
music('battle_dark', {volume:1.0}, function(){
	music('battle_dark_loop');
});
```

h2: 我可不能讓它贏。

```
publish("act3",["roofhunter",25]);
publish("act3-alpha", ["roofhong",0]);
publish("act3-alpha", ["transition",1]);
publish("act3",["dd",6]);
```

r: 這才對嘛，^去他狼的^！我相信你寶貝！殺了它！<3

(#act3a)



# act3a

```
Game.clearText();
publish("act3-out");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
_.act3_bb_body = 1;
```

(...1500)

```
publish("hp_show");
```

b: 別別別別別

n: 這一章有兩個不同結局， 其中一個會 *非常糟。*

b: **別別別別別別別別別別別別**

n: *小心決策， 保護人類。*

`bb({ eyes:"oh_crap", mouth:"normal_talk", MOUTH_LOCK:true });`

b: **啊啊啊啊啊啊啊啊啊啊啊啊**

`bb({ mouth:"normal" });`

n: *祝你好運*

```
Game.clearText();
bb({ eyes:"start" });
```

[你真的可能會_死_！人類！](#act3a_harm) `Game.OVERRIDE_CHOICE_LINE=true`

[這太蠢了！這是自我毀滅！](#act3a_bad) `Game.OVERRIDE_CHOICE_LINE=true`

[那些神經病根本就不是你的朋友！](#act3a_alone) `Game.OVERRIDE_CHOICE_LINE=true`

# act3a_harm

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: **你真**--

(#act3a_after)

# act3a_alone

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: **那些**--

(#act3a_after)

# act3a_bad

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: **這太**--

(#act3a_after)

# act3a_after

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: 你知道嗎，我本來可能會相信你的...要是你沒有把你那套用了千萬遍。

h: 你是那個叫狼來了的大灰狼。

```
bb({ eyes:"sad" });
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act3_fork) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act3_fork) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act3_fork) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`


# act3_fork

```
Game.clearText();
bb({body:"special_attack"});
sfx("charging");
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
Game.FORCE_CANT_SKIP = false;
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: 對，包括這一招。

b: 人類...求求你...

`hong({ eyes:"look_right" });`

h: 哦*很抱歉*我的大救星不贊同我的自我治療辦法。

h: 你個^混蛋^看好了，我們*全都*有辦法讓^你狼的^閉嘴。

`hong({ body:"look_up", eyes:"look_up" });`

h: 有人投入工作。

`hong({ body:"look_down", eyes:"look_down" });`

h: 有人投入約炮，嗑藥，或者是刷他們的臉書推送。

`hong({ body:"normal", eyes:"look_right" });`

h: 還有人投入其他人的懷抱。

`hong({ eyes:"angry" });`

h: 而我要投入那個泳池。

[你喝醉了**那是六層樓下面**。](#act3_bad_1_harm)

[幹你就是這樣感謝我的？！](#act3_bad_1_insult) `bb({eyes:"angry"});`

[ 好吧，我承認，我搞砸了。](#act3_good_1) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_1_harm

b: 就算是你能落在水裡，水面張力**至少**也能讓你摔得粉身碎骨！

h: 呃

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: 我在YouTube上看到有戰鬥民族的人試過了。

(#act3_bad_2)

# act3_bad_1_insult

`hong({ eyes:"look_right" });`

h: 我- 你再說一遍，*感謝*？

`bb({ eyes:"angry" });`

b: 這就是我*存在*的原因啊！因為根本不能去相信人類有能力去保護自己！

b: 這輩子我就做了一件事情那就是讓你避開危險！結果現在你就要這樣--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)

# act3_good_1

`hong({ body:"laugh_1" })``

h: 呵

`hong({ body:"laugh_2" })``

h: 呵呵哈哈哈

`hong({ body:"laugh_3" })``

h: **啊哈哈哈哈哈哈哈哈**

```
bb({ eyes:"sorry"});
hong({ body:"yell_1", mouth:"yell", eyes:"blank" });
```

h: 哇這簡直是這個世紀最^他狼的^輕描淡寫了！

`hong({ body:"yell_2" });`

h: 對沒錯，你這個^死臭爛狼頭^！你把一切都^他狼的^搞砸了！

`hong({ body:"normal", mouth:"angry", eyes:"angry" });`

h: 還有別的評論要發表嗎，明知故問大師？

[但是報復我並不是答案！](#act3_good_1_fail_revenge) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[但是這一次我*真的*是對的！](#act3_good_1_fail_harm) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[我傷害了你。](#act3_good_2a)


# act3_good_1_fail_revenge

b: 你需要和自己的情緒建立更健康的關係，而不是把--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)



# act3_good_1_fail_harm

b: 所以拜託，把手裡的瓶子放下然後我們--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)




# act3_bad_2

`bb({ eyes:"sad" });`

b: 求你了千萬別...

h: 你的血條看來已經見底了，大灰狼。

h: 如果我是你的話，說話會再小心一點，

`bb({ eyes:"normal" });`

[行，我再也不管你了。](#act3_bad_2_jump) `bb({ mouth:"ignore", eyes:"ignore" });`

[我一直都是對的。](#act3_bad_2_right)

[我很抱歉。](#act3_good_2b) `bb({mouth:"sorry", eyes:"sorry_down"});`


# act3_bad_2_jump

b: 行，那你跳吧。看誰管你。

`hong({ eyes:"look_right", mouth:"normal", MOUTH_LOCK:true });`

h: ...

```
hong({ eyes:"less_angry", mouth:"normal" });
bb({ eyes:"ignore_oh_crap" });
```

h: 很好。我先乾杯。

```
bb({ mouth:"normal", eyes:"oh_crap" });
Game.OVERRIDE_TEXT_SPEED = 2;
```

b: **等一下不我剛剛那是反向心理學你應該故意不聽我說**--

(#act3_bad_3)



# act3_bad_2_right

`bb({ eyes:"angry" });`

b: 你*確實*把自己置於了危險的境地。你所謂的朋友*正在*利用你，*你自己*也在利用你所謂的朋友。

`bb({ eyes:"sad" });`

b: 所以，求你了，人類，為什麼就是不相信我？！

h: 因為你從來就沒相信過*我*。

(#act3_bad_3)


# act3_bad_2_terrible

`bb({ eyes:"angry" });`

b: 其他人類都花時間去耐心地訓練他們的守衛狼，去*學習*怎麼和它相處。

b: 而不是去憎惡保護自己的守衛狼！所以為什麼你就不--

`bb({ eyes:"normal" });`

h: 滿口^狼言^。

(#act3_bad_3)



# act3_bad_3

```
music(null);
hong({body:"drink"});
bb({body:"attacked"});
publish("bb_STOP_VIBRATING");
attackBB("100p");
```

(...2000)

```
hong({ body:"normal", mouth:"normal", eyes:"normal" });
bb({ body:"dead" });
```

(...999)

h: *「唯一需要恐懼的東西是恐懼自身。」*

`hong({ body:"look_up", mouth:"happy", eyes:"blank" });`

h: *「不要想太多，要看開！」*

`hong({ body:"normal", mouth:"normal", eyes:"normal" });`

h: 我們這個時代的智者都認為：消極的情緒是不好的！

`hong({ eyes:"less_angry" });`

h: 廢話！所以它們才叫做*消極的*！

b: 人類......求你了......

`hong({ eyes:"normal" });`

h: 我之前說：「我只想擺脫所有這些痛苦。」

h: 我現在做到了，我再也感覺不到痛苦，恐懼，或是焦慮...

h: 我什麼都感覺不到。

`_.a3_ending = "jump";`

(#act3_end)



# act3_good_2a

`bb({mouth:"sorry", eyes:"sorry_down"});`

b: 我之前沉浸在不讓任何東西傷害你的念頭裡，以至於沒有意識到是*我*正在創造傷害。

```
bb({ eyes:"sorry"});
hong({ body:"yell_2", mouth:"yell", eyes:"blank" });
```

h: ^幹你狼的^不會吧。

`hong({ body:"yell_1" });`

h: ^靠^。真的需要這麼久你才能發現嗎？！

`hong({ body:"cry", mouth:"cry", eyes:"blank" });`

h: 你這毛茸茸的笨蛋，本來能為我們避免那麼多的麻煩。為什麼你不能早點意識到呢？...

`_.apologized_for_hurt = true;`

(#act3_good_2q)



# act3_good_2b

`hong({ body:"normal", mouth:"angry", eyes:"look_right" });`

h: ...你很*抱歉*。

`hong({ eyes:"angry", MOUTH_LOCK:true });`

h: ...

h: 抱*什麼*歉？

(#act3_good_2q)


# act3_good_2q

`bb({mouth:"sorry", eyes:"sorry"});`

{{if _.apologized_for_hurt}}
(#act3_good_2q_already_apologized)
{{/if}}

{{if !_.apologized_for_hurt}}
(#act3_good_2q_not_already_apologized)
{{/if}}


# act3_good_2q_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"less_angry" });`

[我很抱歉我沒保護好你。](#act3_good_3_protector)

[我很抱歉我不夠尊重你。](#act3_good_3_respect)

[我很抱歉。](#act3_good_4)


# act3_good_2q_not_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"angry" }, 0);`

[我很抱歉我的人類這麼爛！](#act3_bad_2_terrible) `bb({mouth:"normal", eyes:"normal"})`

[我很抱歉我不夠尊重你。](#act3_good_3_respect)

[我很抱歉我傷害了你。](#act3_good_3_hurt)



# act3_good_3_protector

`bb({eyes:"sorry_down"});`

b: 我的職責是為你警戒*真正的*危險，而不是對著車子和路人狂吠。

`bb({eyes:"sorry_up"});`

b: 衝著陰影狂吠，吠個不停。

`bb({eyes:"sorry"});`

b: 你恨不得給我按上嘴套很正常。

`bb({eyes:"sorry_down"});`

b: 我很抱歉。

(#act3_good_4)



# act3_good_3_respect

`bb({eyes:"sorry_down"});`

b: 我本來應該是*你的*忠誠守衛，但我卻表現得是在要求你聽*我的*命令。

`bb({eyes:"sorry_up"});`

b: 守護者和典獄長本來應該是不同的概念，而我越界了。

`bb({eyes:"sorry_down"});`

b: 我很抱歉。

(#act3_good_4)



# act3_good_3_hurt

`bb({eyes:"sorry_down"});`

b: 我之前沉浸在不讓你受到傷害的念頭裡，從沒有停下來去意識到是*我*正在傷害你。

`bb({eyes:"sorry_up"});`

b: 我是條壞狗狗。

`bb({eyes:"sorry_down"});`

b: 我很抱歉。

(#act3_good_4)


# act3_good_4

```
music(null,{fade:3});
hong({ eyes:"less_angry", MOUTH_LOCK:true },0);
```

h: ...

```
hong({ body:"stop", mouth:"stop", eyes:"blank" });
```

h: 啊，那好吧，反正這本來也不是什麼好主意。

h: 我做這件事本來是想讓你亂了陣腳，然後，嗯，我覺得我做到了。

h: 我們這輪就算平手吧，好嗎？

```
bb({ mouth:"sorry", eyes:"sorry" });
bb({ MOUTH_LOCK:true });
```

b: ...

b: 好。

h: 好。

n: *平手*

`_.a3_ending = "walkaway";`

(#act3_end)









# act3_end

```
Game.clearText();
publish("act3-in");
publish("hp_hide");
Game.FORCE_CANT_SKIP = true;
```

{{if _.a3_ending=="walkaway"}}
(#act3_walkaway)
{{/if}}

{{if _.a3_ending=="jump"}}
(#act3_jump)
{{/if}}






# act3_walkaway

```
publish("start-walkaway-anim");
Game.WORDS_HEIGHT_BOTTOM = 205;
```

(...3501)

```
sfx("bottle_toss");
publish('hong-next');
publish("act3",["roofhunter",7]);
```

(...667)

```
publish("act3",["dd",4]);
publish("act3",["roofhunter",26]);
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("concrete_step2");
```

(...667)

```
publish('hong-next');
publish("act3",["roofhunter",27]);
```

`Game.FORCE_CANT_SKIP = false;`

r: *不會吧*？那個猛獸折磨了你這麼久，結果你就這麼*放棄*了？

r: 你怎麼了小朋友？*害怕*了？

```
publish('hong-next');
publish("act3",["roofhunter",26]);
```

h2: 對。

h2: 我是害怕了。

`publish('hong-next')`

h2: 但是那也沒關係。

`publish('hong-next')`

h2: 感到害怕也沒有關係。

`publish('hong-next')`

(...500)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1167)

```
publish('hong-next');
```

(...833)

```
publish('hong-next');
sfx("rustle2");
```

(...1333)

```
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",31]);
sfx("concrete_step4");
```

(...667)

```
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("door");
```

(...1333)

```
publish('hong-next');
sfx("concrete_step2");
```

(...501)

```
publish('hong-next');
Game.FORCE_CANT_SKIP = false;
sfx("lock_door");
publish("act3",["roofhunter",32]);
```

(...2001)

```
publish("act3",["roofhunter",33]);
```

r: 他剛剛是不是把門給鎖了？

```
Game.clearAll();
_.INJURED = false;
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2000)

(#act4)




# act3_jump

```
publish("start-jump-anim");
Game.FORCE_TEXT_Y = 300;
```

(...2001)

```
publish('hong-next');
sfx("bottle_toss");
```

(...833)

```
sfx("concrete_step1");
sfx("claps");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",28]);
```
(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step2");
publish('hong-next');
publish("act3",["roofhunter",28]);
```

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",34]);
```

(...1167)

```
sfx("rustle2");
publish('hong-next');
```

(...1001)

`publish('hong-next')`

b: 別...

(...501)

`Game.clearText();`

`publish('hong-next')`

(...1333)

```
sfx("quack");
publish('hong-next');
```

(...1333)

`publish('hong-next')`

b: 別別別

(...501)

`Game.clearText();`

`publish('hong-next')`

(...2001)

```
sfx("rustle2");
publish('hong-next')
```

(...501)

```
sfx("concrete_step1");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",30]);
```

(...167)

```
sfx("concrete_step2");
publish('hong-next');
```

(...167)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",2]);
publish("act3",["roofhunter",15]);
```

(...167)

```
sfx("bottle_slip");
publish('hong-next');
publish("act3",["dd",3]);
publish("act3",["roofhunter",16]);
```

(...833)

```
sfx("rustle");
publish('hong-next');
```

(...167)

`publish('hong-next')`

(...167)

```
publish('hong-next');
Game.FORCE_TEXT_Y = 325;
Game.OVERRIDE_FONT_SIZE = 50;
```

b: **不！**

(...400)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-injury-show");
publish("hide_tabs");
```

(...2000)

```
sfx("hospital1");
publish("act4-injury", [1]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital2");
publish("act4-injury", [2]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital3");
publish("act4-injury", [3]);
```

(...8000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...5500)

`_.INJURED = true;`

(#act4)
