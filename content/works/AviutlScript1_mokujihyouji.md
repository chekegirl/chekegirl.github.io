---
title: "【Aviutlスクリプト】『目次表示システム』目次を背景付きで綺麗に表示できるスクリプトとサンプルテーマ"
date: 2023-07-18T04:11:47+09:00
draft: false
categories: [ "素材配布" ]
tags: [ "Aviutlスクリプト", "Aviutl", "目次表示システム", "音街ウナ"]
image: "images/works/AviutlScript1_mokujihyouji/Whole/thumbnail2.png"
type: post
---

目次を良い感じに表示し、さらに背景を良い感じに付ける事ができる[Aviutl](http://spring-fragrance.mints.ne.jp/aviutl/)向けのスクリプト([目次表示システム](https://github.com/chekegirl/AviutlScript_MokujiHyouji/releases/tag/v1.0))を作成しました。

このスクリプトでは、マークダウンと似て非なる記法により目次を体系だった表示にすることが出来ます。

また、背景テーマを読み込むことにより綺麗に背景を自動表示することができます。背景テーマを自分で作る事も手軽に行えます。

ダウンロード： https://github.com/chekegirl/AviutlScript_MokujiHyouji/releases/tag/v1.0

# これは何？何ができるの？

気の利いた背景をつけた状態で、目次を手軽に表示することができる[Aviutl](http://spring-fragrance.mints.ne.jp/aviutl/)向けのスクリプトです。

![目次の例](/images/works/AviutlScript1_mokujihyouji/WhatsThis/mokuji_rei_2.png)

こんな感じで、目次を綺麗に、背景付きで表示できます。

また、

![目次の例](/images/works/AviutlScript1_mokujihyouji/WhatsThis/mokuji_rei2_2.png)

項目番号を変えると、自動で項目を折りたたんだり、背景を調整したりして表示してくれます。

# 導入方法

[Aviutl version1.10](http://spring-fragrance.mints.ne.jp/aviutl/)、[拡張編集version0.92](http://spring-fragrance.mints.ne.jp/aviutl/)に対して目次表示システムを導入する方法について説明します。

## Aviutlと拡張編集Plugin

まず、前提として、[Aviutl](http://spring-fragrance.mints.ne.jp/aviutl/)直下に[拡張編集Plugin](http://spring-fragrance.mints.ne.jp/aviutl/)が存在している状態だとします。

![Aviutlと拡張編集](/images/works/AviutlScript1_mokujihyouji/dounyuu/AviutlAndExedit.png)

もし他のファイル構成であれば、それに応じた形でこれ以降の文章を読み替えてください。

ここに、``script``フォルダが無ければ、作ります。

![scriptフォルダ](/images/works/AviutlScript1_mokujihyouji/dounyuu/script_fold.png)

## rikky_moduleの導入

このスクリプトを用いるには[rikkymodule&memory](https://hazumurhythm.com/wev/amazon/?script=rikkymodulea2Z)が必要です。[rikkymodule&memory](https://hazumurhythm.com/wev/amazon/?script=rikkymodulea2Z)をダウンロードし、解凍したら、導入します。

![rikkymodule](/images/works/AviutlScript1_mokujihyouji/dounyuu/rikky_module_dounyuu.png)


## 目次表示システムの導入

あとは、``script``フォルダ内に[目次表示システム](https://github.com/chekegirl/AviutlScript_MokujiHyouji/releases/tag/v1.0)を貼り付けます。

ダウンロード： https://github.com/chekegirl/AviutlScript_MokujiHyouji/releases/tag/v1.0

![目次表示anm](/images/works/AviutlScript1_mokujihyouji/dounyuu/MokujiSystemToScript.png)

これで導入は完了しました。

# 目次を表示するまで

目次表示システムを導入した後、目次を実際に表示する方法について説明します。

## スクリプトの適用

Aviutlのテキストオブジェクトを用います。

ここに、アニメーション効果を追加し、目次表示を選択します。

![目次表示適用](/images/works/AviutlScript1_mokujihyouji/HyoujiMade/TextAnimation.png)

## 目次テキストを書く

目次はテキスト欄に次のように書く必要があります。

``[インデントの下がり幅分の#][半角Space][項目文字列]``

例として次のように書いたとします。

```
項目１
# 項目１ー１
## 項目１ー１ー１
## 項目１ー１ー２
## 項目１ー１ー３
# 項目１ー２
## 項目１ー２ー１
## 項目１ー２ー２
## 項目１ー２ー３
# 項目１ー３
## 項目１ー３ー１
## 項目１ー３ー２
## 項目１ー３ー３
項目２
# 項目２ー１
## 項目２ー１ー１
## 項目２ー１ー２
## 項目２ー１ー３
# 項目２ー２
## 項目２ー２ー１
## 項目２ー２ー２
## 項目２ー２ー３
# 項目２ー３
## 項目２ー３ー１
## 項目２ー３ー２
## 項目２ー３ー３
```

これで「項目」というパラメータを3にしてみると、次の画像のように表示されるはずです。

![目次表示背景なし](/images/works/AviutlScript1_mokujihyouji/HyoujiMade/NoBackImage.png)

## 背景テーマを使用する場合

「設定」から「背景を表示する」にチェックを入れます。

![目次表示背景表示](/images/works/AviutlScript1_mokujihyouji/HyoujiMade/BackImageCheckSys.png)

「背景フォルダ」ボタンをクリックし、背景テーマのフォルダを選択します。

![目次表示背景選択](/images/works/AviutlScript1_mokujihyouji/HyoujiMade/ChooseFoldSys.png)

ここで、パラメータを良い感じに設定してみると...

![目次表示Param](/images/works/AviutlScript1_mokujihyouji/HyoujiMade/ParamSetSys.png)

これで、次のように表示されるはず。

![目次背景付できた～](/images/works/AviutlScript1_mokujihyouji/HyoujiMade/BackImagePlusAll_2.png)

# 目次表示システムを使う際の設定項目

目次表示を行った後、表示内容を調整したくなった際に弄る設定項目について説明します。

## Aviutl上で設定できる部分

表面に出ている部分で設定できる内容はこのようになっています。

| 項目名       | 設定内容      |
|:-----------:|:------------:|
| 項目        | テキスト欄に記載した項目のうちどの項目を選択するかを表す番号。 |
| ｲﾝﾃﾞﾝﾄ      | インデント1つの深さを表す数字。大きいほど深い。       |
| 深度ｻｲｽﾞ    | インデントが1つ深くなるごとに文字の大きさが何%大きくなるかを表す数字。マイナスの場合は小さくなる。 |
| 選択サイズ  | 選択されている項目及びその親項目の文字の大きさが何%大きくなるかを表す数字。マイナスの場合は小さくなる。 |

また、「設定」から設定できる内容はこのようになっています。
| 項目名        | 設定内容      |
|:-------------:|:------------:|
| 選択文字色     | 選択されている項目及びその親項目の文字の色 |
| 選択文字縁色   | 選択されている項目及びその親項目の文字の縁取りや影の色 |
| 上位項目を含む | 選択されている項目の親項目を強調表示するかどうか |
| 折りたたむ     | 選択されている項目及びその親項目、またそれらと並列な関係にある項目以外を表示するかどうか |
| 背景を表示する | 背景の模様を表示するかどうか |
| 背景右長さ     | 背景画像の横幅。この数字を大きくすると左端は変わらず右端が右に行く |
| 背景フォルダ   | 背景テーマのフォルダ。いくつかの画像とsetting.iniから成るフォルダを選択する |
| 枠左余白       | 背景の目次の文字のに対する左の余白 |
| 枠上余白       | 背景の目次の文字のに対する上の余白 |
| 枠下余白       | 背景の目次の文字のに対する下の余白 |

背景フォルダ以外の項目は基本的に弄ってみるのが手っ取り早いです。

## 設定ファイルを編集する必要がある部分

Aviutl上で設定できる項目とは別に、背景テーマのsetting.iniを編集することで設定可能な項目も存在します。これらは背景テーマを作る際に設定するものですが、Aviutl上でテーマを使用する人間が弄る事も考えられる項目がいくつか存在するので、それらを紹介します。

| 項目名        | 設定内容      |
|:-------------:|:------------:|
| PatchPosition[XorY][数字] | 背景テーマの"one_point[数字].png"の表示される位置を変える。[XもしくはY]がXなら"Right","Mid","Left"、Yなら"Ceil","Mid","Floor"で設定する。 |
| PatchOffset[XorY][数字] | 背景テーマの"one_point[数字].png"の表示される位置を変える。数字で指定する。PatchPositionで指定した場所からX方向Y方向にそれぞれどれほど動かすかを指定している。 |
| RuledLineOffsetY | 罫線の文に対するY方向(高さ方向)の位置を変える。数字で指定する。 |

特に最後のRuledLineOffsetYについては、フォントに応じて変える必要が出てくるものと考えられますね。じゃあなんでAviutl上で設定できるようにしなかったかというと、なんか設定項目に含めたら動かなくなったので...

# 背景テーマ素材の作成方法

背景のテーマを自分で作成する方法を説明します。対称定規が使えるお絵描きソフト(クリスタなど)があると便利かも...

## 背景画像に関する仕様

背景テーマ全体として、角、枠、背景の３つは、次の画像のように表示されるようになっています。

![背景のテーマ全体の図](/images/works/AviutlScript1_mokujihyouji/ThemeMake/BackThemeFigure.png)

また、罫線は常に文字の下に位置を合わせて表示されます。

更に、Patchとして複数の画像を表示することができます。Patch画像は背景画像の範囲内でのみ表示され、はみ出す分についてはクリッピングされます。

これらの画像は、``背景 → Patch → 枠 → 角 → 罫線``、という順番で貼り付けられています。また、背景テーマのフォルダ直下に、全ての使用する画像を置く必要があります。

## 設定ファイルの書き方

背景テーマを作る上で、設定ファイルを書く必要があります。設定ファイルの名前は``setting.ini``である必要があります。また、背景テーマのフォルダ直下に置く必要があります。

設定ファイルは``[設定項目名] = [設定値]``という行を繰り返す形で書きます。

### 背景画像に関する設定項目

| 項目名        | 設定の種類    |
|:-------------:|:------------:|
| BackImageType | None : 背景画像なし <br> LongClip : 背景画像を目次の範囲に合わせて切り抜く <br> Resize : 背景画像全体を目次の範囲に合わせて伸縮 |
| BackImagePosition <br> (BackImageType = LongClipのときのみ)  | LeftCeil : 左上合わせ <br> LeftFloor : 左下合わせ <br>  RightCeil : 右上合わせ <br> RightFloor : 右下合わせ |

### Patch画像に関する設定項目

| 項目名        | 設定の種類    |
|:-------------:|:------------:|
| PatchQuantity | 非負整数 : Patch画像の数 |
| PatchPositionX[n] <br> ([n] ≦ PatchQuantity) | Right : X座標の端は右合わせ <br> Mid : X座標の端は真ん中合わせ <br> Left : X座標の端は左合わせ |
| PatchPositionY[n] <br> ([n] ≦ PatchQuantity) | Ceil : Y座標の端は上合わせ <br> Mid : Y座標の端は真ん中合わせ <br> Floor : Y座標の端は下合わせ |
| PatchOffsetX[n] <br> ([n] ≦ PatchQuantity) | 整数 : Patch画像がPatchPositionX[n]からどれだけズレた位置か |
| PatchOffsetY[n] <br> ([n] ≦ PatchQuantity) | 整数 : Patch画像がPatchPositionY[n]からどれだけズレた位置か |
| PatchOverLine[n] <br> ([n] ≦ PatchQuantity) | True : Patch画像と被る位置の罫線を打ち消す <br> それ以外(普通はFalse) : Patch画像と被る位置の罫線を打ち消さない |

### 枠画像に関する設定項目

| 項目名        | 設定の種類    |
|:-------------:|:------------:|
| FrameType     |  None : 枠画像なし <br> LongClip : 枠画像の長さを目次の範囲に合わせて切り抜く <br> Resize : 枠画像の長さを目次の範囲に合わせて伸縮 <br> Recursive : 枠画像を目次の範囲に合わせて繰り返し並べて表示|

### 角画像に関する設定項目

| 項目名        | 設定の種類    |
|:-------------:|:------------:|
| CornerType    |  None : 角画像なし <br> Raw : 角画像あり |

### 罫線画像に関する設定項目

| 項目名        | 設定の種類    |
|:-------------:|:------------:|
| RuledLineType | None : 罫線画像なし <br> LongClip : 罫線画像の長さを目次の幅に合わせて切り抜く <br> Resize : 罫線画像の長さを目次の幅に合わせて伸縮 <br> Recursive : 罫線画像を目次の幅に合わせて繰り返し並べて表示|
| RuledLineOffsetY | 整数 : 罫線画像が通常時からどれだけY方向にズレた位置か |


## 背景テーマ作成時のコツ

背景テーマを作成する際は、背景全体をまずは1枚の画像として作ってから、適切に画像を切り分けると作りやすいことが多いです。（少なくとも僕はその方が作りやすかったです。）

また、あまり厳密に考えすぎず、とりあえず作ってみると良いです（厳密に考え出すとピクセル数を数えるような事になってとてもつらいので）

