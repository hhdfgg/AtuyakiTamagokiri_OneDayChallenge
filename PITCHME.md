![GIF](/1515170556427.gif)

---
作製時間　約22時間

---
### <font color="Black">操作方法</font>
２つの<font color="Red"><b><u>ゲージ</u></b></font>を<font color="Red"><b><u>タイミング良くクリック！</u></b></font>  

---
### <font color="Black">ゲーム説明</font>  
２つの<font color="Red">ゲージ</font>で厚焼き玉子を斬る<font color="Blue">スピード</font>が変わる
<font color="SlateBlue">スコア</font>は厚焼き玉子を<font color="SlateBlue">何個斬れたか</font>

---

<b>要するに、<font size="20" color="Blue"><u>瓦割</u></font>です</b>

---
[厚焼き！玉子斬りッッッ(GitHubPages)](https://hhdfgg.github.io/AtuyakiTamagokiri_OneDayChallenge/)

https://hhdfgg.github.io/AtuyakiTamagokiri_OneDayChallenge/


[厚焼き！玉子斬りッッッ(unityroom)](https://unityroom.com/games/atuyaki_oneday)

https://unityroom.com/games/atuyaki_oneday

---
### <font color="Black">使用素材</font>  
#### アセットストア
- [Greatsword of Frozen Night](https://www.assetstore.unity3d.com/jp/#!/content/28991)
- [TextMesh Pro](https://www.assetstore.unity3d.com/jp/#!/content/84126)  
- [UniRx-Reactive Extensions for Unity](https://www.assetstore.unity3d.com/jp/#!/content/17276)(ほんの一部分)

---
#### BGM・効果音/フォント  
- [HURT-RECORD](http://www.hurtrecord.com/)  
- [効果音ラボ](https://soundeffect-lab.info/)  
- [フリー効果音素材 くらげ工匠](http://www.kurage-kosho.info/)  
- 源界明朝

---
#### <font color="Black">参考サイト</font>
[テラシュールブログのトランジション](http://tsubakit1.hateblo.jp/entry/2015/11/04/015355)
- Fade Camera  
- マスク画像[For you](http://4you.bz/)
 
[テラシュールブログのパーティクルで紙ふぶきを散らす](http://tsubakit1.hateblo.jp/entry/2015/09/04/233000)

---
[【Unity、WebGL】なるべく簡単にオンラインランキング機能をつけるサンプル](http://blog.naichilab.com/entry/webgl-simple-ranking)

- [ニフクラ mobile backend](http://mb.cloud.nifty.com/doc/current/introduction/quickstart_unity.html)

(NCMB・ニフティクラウド)
 
[【Unity C#】関数を1回だけ呼ぶ方法](https://qiita.com/r-ngtm/items/fe27b49f4156bfbe2b9e)のUniRx

---
### <font color="Black">トランジション<font>
#### (フェードイン、フェードアウト、ワイプ、オーバーラップなど切り替え効果のこと)

この記事は2015年11月4日でちょっと古く、少し設定が違うのですが、

ざっくり言うと、たぶん

---
<b><font color="Blue">Fade Cameraによって、白黒の画像をアルファチャンネルに変換してエフェクトをかけている</font></b>

ってことだと思います。

---
<b>ほんの一部分だけ使ってみた<font size="15" color="Red"><u>UniRx</u></font></b>

- Update内で関数を1回だけ呼びたいと思って調べてみたら  |

---

```cs
using UniRx;
using UniRx.Triggers;

// 省略

// Time.time > 1.5f の場合に１回だけHoge()を実行
this.UpdateAsObservable().First(x => Time.time > 1.5f).Subscribe(x => Hoge());

```

---
このような書き方で動作するらしい！

ってことで、やってみたら、ちゃんと動作しました！

でも、あまりよくわかっていないですが、調べて、　どんどん使っていきたい

---
### <font color="Black">最後に</font>

---
夏休みよりも確実に成長できているなと実感しました！

分からないことの調べ方だったり、アセット使い方だったり、

---
でも、実感はしたけど満足はしていないので、

まだまだ努力していきたいと思いました。
