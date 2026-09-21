#  【read me】  grand-circle

## 用字用語
- お土産
- わかる
- 飴
- 入り口

## 注意
- 写真やGoogle mapの埋め込みの前後にbrを置くとうまく表示できないので、brのない空行で改行する
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
<div style="position: relative; width: 100%; max-width: 315px; padding-bottom: min(560px, 177.78%); height: 0; margin: 0 auto;"><iframe src="https://www.youtube.com/embed/j6AQ2xwHcv0" title="Devil's Bridge駐車場" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0;" allowfullscreen></iframe></div>

*Devil’s Bridge駐車場 ・どうしたらいいかわからない・・・*<br>
<br>
```


divとキャプションの間は空行を1行あける。<br>
iframeの直後にキャプションを続けると、HTMLブロックの一部として扱われ、＊…＊ がイタリックにならず、アスタリスクがそのまま表示される可能性がある。<br>
<br>

## YouTube動画の埋め込み（通常動画）
``` HTML
<div style="position: relative; width: 100%; padding-bottom: 56.25%; height: 0; overflow: hidden;"><iframe src="https://www.youtube.com/embed/zZ_uUisgjxA" title="Scenic Byway 12・The Hogback" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0;" allowfullscreen></iframe></div>

*Scenic Byway 12・The Hogbackをスミーが動画撮影*<br>
```

divとキャプションの間は空行を1行あける。<br>
iframeの直後にキャプションを続けると、HTMLブロックの一部として扱われ、＊…＊ がイタリックにならず、アスタリスクがそのまま表示される可能性がある。<br>
<br>

## ページリンク
``` markdown
[【グランドサークル】　1日目　羽田 〜 Sedonaへ](day01.html)
```

## Googleなどの検索エンジンに引っかからないようにする
- robots.txtに検索エンジンに引っかからないようにコマンドを設定
- 直下に置く
- この処置をしておくと、URLを知っている人しか実質、見られないことになる
- パスワードなどでロックをかけるのは実用的ではなく、無料ツールでやるには無理があるので、この方法がベター

``` Markdown
User-agent: *
Disallow: /
```
