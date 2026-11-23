# macOS版Safariでの設定と適用範囲

ChromeやFirefoxでは、インストールしたフォントを既定フォントに指定できます。この設定は、ブラウザの既定フォントに任せた箇所に適用されます。サイトが独自にフォントを指定した箇所は、そのフォントで表示される場合があります。 [Chromeの設定](https://support.google.com/chrome/answer/96810?hl=ja)・[Firefoxの設定](https://support.mozilla.org/ja/kb/change-fonts-and-colors-websites-use)

macOS版Safariの設定には、既定フォントを選ぶ項目がありません。「詳細」からユーザースタイルシート（CSS）を指定できます。Safariのプライバシー保護機能により、ページから利用者が追加したフォントの参照が制限される場合もあります。青磁の配布ZIPに含まれるCSSには、書体ごとにRegularとBoldのフォントを埋め込んであります。 [Safariの詳細設定](https://support.apple.com/en-ie/guide/safari/ibrw1075/mac)・[WebKitのプライバシー保護](https://webkit.org/tracking-prevention/)

## CSSを指定する

1. [青磁 0.300の配布ZIP](https://github.com/metasta/seiji-fonts/releases/tag/v0.300) を展開します。
2. Safariの「設定 → 詳細 → スタイルシート → その他」で、ZIPの `Safari` フォルダにあるCSSを一つ選びます。
3. 表示するページを再読み込みします。元の表示に戻す場合は、「スタイルシート」を元の設定に戻します。

| 書体 | CSS |
| --- | --- |
| 青磁明朝 | `SeijiMincho.css` |
| 青磁ゴシック | `SeijiGothic.css` |
| 青磁丸ゴシック | `SeijiMaruGothic.css` |

## どの部分に適用されるか

CSSは、日本語と指定された本文、見出し、表、ルビなどを対象にします。対象の要素にサイトがフォントを指定した場合も、このCSSの指定が優先します。ただし、対象の内側にある別の要素にサイトが個別のフォントを指定した場合など、その部分はサイトのフォントで表示されることがあります。 [CSSでの指定の優先順位](https://www.w3.org/TR/css-cascade-5/#cascade-origin)

ナビゲーション、コード、ボタンや入力欄などは、このCSSで直接指定する対象から外れます。青空文庫の旧形式のページでは、サイトの情報と日本語の指定をもとに、本文を対象とします。

表示を確認するには、青空文庫『三国志 図南の巻』を開きます。冒頭の「帰」が「歸」の字形で表示されます。 [青空文庫『三国志 図南の巻』](https://www.aozora.gr.jp/cards/001562/files/52417_51068.html)

## 青磁で表示されない場合

ページの言語指定やフォントの読み込み条件によっては、CSSの指定が反映されない場合があります。一部の漢字だけ別の書体で表示される場合は、配布ZIPの `収録漢字.txt` でその字の有無を確認できます。 [漢字の収録範囲](coverage.md)

青磁を更新する場合は、Safariの設定で新しい版のCSSを選び、ページを再読み込みします。
