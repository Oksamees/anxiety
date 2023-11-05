# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[MÄNGI!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Niisis, enne kui alustame, kuidas *sulle* meeldiks teksti lugeda?

`publish("show_options_bottom")`

# intro-start-2

n3: Alustagem siis meie lugu...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: SEE ON INIMENE

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

n: JA SEE ON INIMESE ÄREVUS

n: _SINA_ OLED ÄREVUS

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Eih. Ei, ei, ei kuula. Vaatan oma telefoni.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: SU ÜLESANNE ON KAITSTA OMA INIMEST *OHU EEST*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Ohh! Sa raiskad enda elu Twitteris skrollimise peale, jälle!


```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Jah, ma imestan küll, miks ma ei istuks lihtsalt ning oma mõtteid sagedamini kuulaks. 

`hong({eyes:"neutral"});`

n: KIIRESTI, HOIATA TEDA *OHUST!*

```
bb({eyes:"look"});
```

[Oi, vaata seda jubedat uudist!](#act1d_news)

[Oh ei, kas see säuts on salaja *meie kohta?*](#act1d_subtweet)

[Hei, GIF kiisust, kes joob piima](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: HEH jah, see on tõesti armas, ma--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: KASSID EI SUUDA PIIMA SEEDIDA NING ME OLEME KOHUTAVAD INIMESED, KUNA NAUDIME LOOMADE VÄÄRKOHTLEMIST

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



