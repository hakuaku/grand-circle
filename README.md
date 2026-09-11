#  【read me】  grand-circle

## 用字用語
- お土産
- わかる
- 飴

## 注意
- 写真やGoogle mapの埋め込みの前後に<br>を置くとうまく表示できないので、<br>のない空行で改行する
- 文章の途中で読みやすさを考慮して改行を入れると、デバイスによってものすごく読みにくくなるので 一つの文章内で改行はせず、CSSファイルで表示幅を720pxに設定する
- CSSファイル
    - assets/css/style.scss
    - 720px幅で折り返すように設定

## 写真
- 写真幅：1600px
- 写真解像度：72dpi
- ファイル名：day⚫︎-連番-内容.jpeg
- iPhoneで撮影した写真の拡張子はHEIC
- iPhoneからMacBookへAirDropで写真を転送
- ツール>サイズの変更　：解像度を下げる
- ファイル>書き出し　　：拡張子をJPEGに変える

``` Markdown
![Delicate Arch・Delicate Arch Trailの看板](images/day07-01-delicate-arch-morning.jpeg)
*Delicate Arch・Delicate Arch Trailの看板*<br>
<br>
```

## コラム
``` HTML
--- 
<div style="border: 1px solid #ccc; padding: 16px; margin: 16px 0;"> 

**📖 コラム｜キャニオンスピリット（Canyon Spirit）** <br>
<br>
カナダの豪華観光列車「ロッキーマウンテニア」を運営するArmstrong Collectiveが手がける、アメリカ南西部の新しい高級観光列車。<br>

 </div>
--- 
```

## 本日の移動
```
📍 **本日の移動** <br>
羽田 → サンフランシスコ → フェニックス → アズビルノースアメリカ → Walmart → REI → Desert Vista → Robbers Roost → Sedona / SAFEWAY → Greentree Inn Sedona
```

## Google map埋め込み
- Google mapで対象となる地点を表示
- [共有]
- [地図埋め込む]
- [HTMLをコピー]
- width=“100%”で設定

``` HTML
<iframe src="https://www.google.com/maps/embed?pb=!4v1784533761787!6m8!1m7!1sCAoSF0NJSE0wb2dLRUlDQWdJRFdwcHZBalFF!2m2!1d38.73573150781716!2d-109.5203161864834!3f270!4f0!5f0.7820865974627469" width="100%" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="strict-origin-when-cross-origin"></iframe>
```

## YouTube動画の埋め込み（ショート動画）
- URLのYouTubeの下はembedにする

``` HTML
<iframe width="315" height="560" src="https://www.youtube.com/embed/9YkbzdosDNE" frameborder="0" allowfullscreen> </iframe>
```

## YouTube動画の埋め込み（通常動画）
``` HTML
<iframe width="560" height="315" src="https://www.youtube.com/embed/zZ_uUisgjxA" title="YouTube video player" frameborder="0" allowfullscreen></iframe>
```

## ページリンク
``` markdown
[【グランドサークル】　1日目　羽田 〜 Sedonaへ](day01.html)
```
