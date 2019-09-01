# こういうのたのしい

なんか謎に色ついてないとこあるし(公式でも)自分の好きな色で作ってみようかなっておもい、  
`Visual Studio Code` のカラーテーマを自作しました。  
特にシンタックスハイライトはこだわるとめっちゃ時間がかかるので、もとからあるテーマを編集するののほうが良かったかもとおもいつつ、やはり自分でイチから作ったほうがなんやかんや精神的にもええなっておもいました。(思想が強い)  
エディタってめっちゃ使うしな  


## 色

![my-iro](readmeImage/my-iro.png)

### 白　　(#FFF)
記号(括弧,演算子...),HTMLのタグ中の文字

### 黄緑　(#9F6)
Class,型,HTMLタグ名,CSSセレクタ

### 青緑　(#3CC)
変数,プロパティ,HTML属性名,CSSプロパティ,key

### 橙　　(#F93)
関数,メソッド

### 黃　　(#FF6)
文字列,value

### 桃　　(#F9F)
識別子,言語構造,制御構造

### 紫　　(#96F)
真偽,空,数,定数

### 深緑　(#060)
コメント

## 手順
ほぼ下のリンクを習って。。。  
1. 下にある`TmTheme Editor`で大体をつくってダウンロード
1. ターミナルで `npm install -g yo generator-code` (すでにNode入っている前提)
1. ターミナルで `yo code`
1. ミスってなんかを押したのかよくわからなくなったので `control + C` でもいっかい2
1. 矢印キーで`New Color Theme`選びEnter
1. 名をいれてってEnter
1. ダウンロードした`.TmTheme`のパスを選ぶときに選ぶ
1. 作ってくれる
1. `/themes`中のjsonファイルをいじっていく
1. それ見てみてください
1. ソフトウェア自体の色は色々ありますが、シンタックスハイライトは何色か決めてその中で適応したいコードをみて追加変更して行きたかったので色でまとめる形を取っていくように変更しました。
2. `/Users/{ユーザー名}/.vscode/extensions/`にフォルダごとぼんって入れる。パッケージ自体をあれしてるjsonもあるので
3. したら `command + K -> comand + T` でカラーテーマえらべるね！
4. `command + shift + P` で`tm`と検索、`開発者: TMスコープの調査(Developer: Inspect TM scopes)`を使ってシンタックスハイライトのための要素を調査できる。細かく指定するほど、競合した際に強い指定になる。
5. `command + shift + P` で`re`と検索、`Developer: ウィンドウ再読み込み(Deveoper: Reload Window)`を使って再読み込みすると反映したテーマを確認できる。(なんでこっちは開発者ではないのか)

## 雑記
- いちからつくる
- `/themes`中のjsonファイルにつらつらと何を何色にするかかいていく
- `#3CC`、suki
- `#FF6`mosuki
- 白黒以外はWebセーフカラーにしてみましたね
- `なんやらbody`ってやつはそれの中身全部染まってまうから超いらん(色つける際のスコープの話です)(括弧も染まっまう)
- Pythonのサポート薄くないですか
- Elmのことめっちゃ忘れてた
- Javaのオブシコしてない頃の変数とがあるのが扱い困る
- 思想は常に変わっていきそう(主に己の知識とか考え方で)
- 言語ごとに絞って適応させたほうが幸せになれるような
- いやJavaもなんかサポ薄いわ
  - それはその言語を書くモチベにかかわる
- ターミナルは鬼黒と鬼緑で別世界感だすね
- 左3つのゆめかわポップ感
  - そっちはピンクとか紫主体よね(虹色角羽馬)
  - オレンジとか緑は非それ
- システムに近い色は(?)そのままにしておいています(めんどくさいからじゃないですからね←)
- HTML,CSS(SCSS),JS(TS),ELM,PHP,PYTHON,JAVAはしたいね
- HTMLのタグ名やCSSのセレクタはClassではないか<-???????
- HTMLのinnerは文字列なんやけどほぼ慣習的に白みたいなとこある。タグ自体のとかぶるのは良くないしえ

## 参考

- [大参考Qiita様](https://qiita.com/JunSuzukiJapan/items/1f19b440ad1d33cf4421)
- [大本つくってくやつ(.TmTheme)](http://tmtheme-editor.herokuapp.com)
- [公式のつくりかた](https://code.visualstudio.com/api/language-extensions/syntax-highlight-guide)
- [公式のトークン集](https://code.visualstudio.com/api/references/theme-color)
- [ちょっと日本語でしてくれてる記事](https://qiita.com/deren2525/items/6bc099ae8c05e3076055)
- [Webセーフカラー超いい感じサイト](http://isseki.dip.jp/usr/public/ColorChart/WebSafeColor.html)
- [6色まで色を並べて見れるサイト、そしてmy-iro](https://colorkitty.com/?colors=33cccc-ffff66-ff99ff-99ff66-ff9933-9966ff)

---
```
     _-----_     ╭──────────────────────────╮
    |       |    │  ika,                    │
    |--(o)--|    │  watashi ga tsukutta     │
   `---------´   │  README desu.            │
    ( _´U`_ )    ╰──────────────────────────╯
    /___A___\   /
     |  ~  |     
   __'.___.'__   
 ´   `  |° ´ Y ` 
```
---


# README
## This is the README for your extension "actionpterygiicolortheme"
You can author your README using Visual Studio Code.  Here are some useful editor keyboard shortcuts:

* Split the editor (`Cmd+\` on macOS or `Ctrl+\` on Windows and Linux)
* Toggle preview (`Shift+CMD+V` on macOS or `Shift+Ctrl+V` on Windows and Linux)
* Press `Ctrl+Space` (Windows, Linux) or `Cmd+Space` (macOS) to see a list of Markdown snippets

### For more information
* [Visual Studio Code's Markdown Support](http://code.visualstudio.com/docs/languages/markdown)
* [Markdown Syntax Reference](https://help.github.com/articles/markdown-basics/)

**Enjoy!**


