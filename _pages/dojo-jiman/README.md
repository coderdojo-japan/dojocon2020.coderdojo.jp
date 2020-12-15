# Dojo自慢掲載マニュアル
お世話になっております。Dojo自慢のデータ記入方法についてこちらでご案内いたします。

## ページ上部の---の中身

jekyllでは--- ---の中で変数とかを貯めておけます。

```
---
layout: jiman_media
title:  "タイトル〜サブタイトル〜（YouTube）"
dojo_name:  "道場名"
thumbnail: jiman/hoge1.png
dojo_desciption: >
  ああああああああああ
dojo_icon:
permalink: /dojo-jiman/fuga/
---
```

1. Layout
  ``jiman_text``と``jiman_media``の2種類をご用意しています。違いとしてはOGP・サムネイルとページ上部に出る画像が共通化されてるのが``jiman_text``，ページ上部に出ないのが``jiman_media``です。これ以外を選ぶとリストに表示されなくなります。
2. Title
  要するに上に出るタイトルです
3. Thumbnail
  ogpのための画像です。``jiman_text``の場合はページ上部に出る画像でもこれが使われます。選ばなかった場合はOGP用の画像が使われます。
4. dojo_name
  Dojoの名前です。ロゴ横に表示されます。
5. dojo_description
  ページ下部にある道場名の下に表示されるものです。
6. dojo_icon
  アイコンです。``coderdojo.jp``から吸いだしています。なお，岡南がOkayamaと指定されているように，道場名と異なるものが指定されている場合がありますので，[``coderdojo.jpレポジトリ/public/img/dojos``](https://github.com/coderdojo-japan/coderdojo.jp/tree/master/public/img/dojos)をご参照ください。
7. permalink
  ``/dojo-jiman/（名称とか番号とか）``と指定してください。

という感じでお願いします。

## ページ中身について
私の環境だけかもしれないですが，HTMLのタグをmarkdownで使うとエラーが起きるので，YouTubeとかを埋め込む際はHTMLを書いてください。