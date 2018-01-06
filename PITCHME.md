![GIF](/1515170556427.gif)

---
作製時間　約22時間

---
### 操作方法  
２つの<font color="Red"><b><u>ゲージ</u></b></font>を<font color="Red"><b><u>タイミング良くクリック！</u></b></font>  

---
### ゲーム説明  
２つの<font color="Yellow">ゲージ</font>で<u>厚焼き玉子を切る</u><font color="Orange">スピード</font>が変わる
<font color="SlateBlue">スコア</font>は<u>厚焼き玉子</u>を<font color="SlateBlue">何個切れたか</font>

---
### 使用素材
#### アセットストア
- [Greatsword of Frozen Night](https://www.assetstore.unity3d.com/jp/#!/content/28991)
- [TextMesh Pro](https://www.assetstore.unity3d.com/jp/#!/content/84126)  
- [UniRx-Reactive Extensions for Unity](https://www.assetstore.unity3d.com/jp/#!/content/17276)(ほんの一部分)

---
#### BGM・効果音/フォント  
- [HURT-RECORD](http://www.hurtrecord.com/)  
- [効果音ラボ](https://soundeffect-lab.info/)  
- [フリー効果音素材 くらげ工匠](http://www.kurage-kosho.info/)  
- [源界明朝](https://www.flopdesign.com/blog/font/5146/)

---
#### 参考サイト
[テラシュールブログのトランジション](http://tsubakit1.hateblo.jp/entry/2015/11/04/015355)
- Fade Camera  
- マスク画像[For you](http://4you.bz/)
 
[テラシュールブログのパーティクルで紙ふぶきを散らす](http://tsubakit1.hateblo.jp/entry/2015/09/04/233000)

---

[【Unity、WebGL】なるべく簡単にオンラインランキング機能をつけるサンプル](http://blog.naichilab.com/entry/webgl-simple-ranking)

- [ニフクラ mobile backend](http://mb.cloud.nifty.com/doc/current/introduction/quickstart_unity.html)
 
[【Unity C#】関数を1回だけ呼ぶ方法](https://qiita.com/r-ngtm/items/fe27b49f4156bfbe2b9e)の3.UniRxを使う

---
### トランジション
#### (フェードイン、フェードアウト、ワイプ、オーバーラップなど切り替え効果のこと)

この記事は2015年11月4日でちょっと古く、少し設定が違うのですが、ざっくり言うと

<b><font color="Blue">Fade Cameraによって、白黒の画像をアルファチャンネルに変換してエフェクトをかけている</font></b>

ってことだと思います。

---
<b>ほんの一部分だけ使ってみた<b><font color="Red"><u>UniRx</u></font></b></b>

Update内で関数を1回だけ呼びたいと思って調べてみたら 

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

---


