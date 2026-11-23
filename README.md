# 青磁 / Seiji

[English](README.en.md)

青磁（せいじ）は、一点明朝正字を基準に漢字の字形を選んだ日本語書体です。青磁明朝・青磁ゴシック・青磁丸ゴシックに、それぞれRegularとBoldがあります。

[フォントをダウンロード](https://github.com/metasta/seiji-fonts/releases)

![青磁明朝・青磁ゴシック・青磁丸ゴシックのRegularとBoldで「夕暮れの驛で友を待つ。」を並べた横組みの見本](seiji-specimen.png)

## 利用方法

### Wordなどのアプリ

配布ZIPを展開し、利用する書体のOTFをインストールします。RegularとBoldを併用する場合は、両方のOTFをインストールします。アプリのフォントメニューで、書体名を選びます。

| 書体 | 英語の表示名 |
| --- | --- |
| 青磁明朝 | Seiji Mincho |
| 青磁ゴシック | Seiji Gothic |
| 青磁丸ゴシック | Seiji Maru Gothic |

### macOS版Safari

「設定 → 詳細 → スタイルシート → その他」で、配布ZIPの `Safari` フォルダにあるCSSを一つ指定し、対象のページを再読み込みします。日本語と指定された本文・見出し・ルビなどに適用されます。 [CSSの選択と適用範囲](docs/safari.md)

## 収録範囲

増補先行版 0.300は、教育漢字1,026字と、教育漢字以外の常用漢字400字を収録します。6本のフォントに共通する計1,426字です。個々の漢字は、配布ZIPの `収録漢字.txt` で確認できます。

## 文脈による字形選択と入力字の指定

「辯」「辨」「瓣」は、今の表記では同じ「弁」と書く別の漢字です。OpenTypeの `calt` が有効な組版環境では、「弁論・弁別・花弁」を「辯論・辨別・花瓣」の字形で表示します。

単独の「弁」は通常「辯」の字形で表示します。「弁」そのものの形が必要なときは、異体字シーケンス（IVS）に対応する環境で、「弁」に異体字セレクタを続けた `弁󠄀` を入力します。0.300でこの指定ができるのは、対応表に記した13組です。 [文脈規則とIVSの対応表](docs/contextual-forms.md)

## 技術資料

- [漢字とかなの収録範囲](docs/coverage.md)
- [漢字の選定基準と青磁の字形](docs/glyph-selection.md)
- [文脈による字形選択と異体字シーケンス](docs/contextual-forms.md)
- [macOS版Safariでの設定と適用範囲](docs/safari.md)
- [既知の表示上の制約](docs/known-issues.md)

## 使用許諾と素材

OTF版のフォントとSafari用CSS内のフォントは、SIL Open Font License 1.1で配布します。著作権表示とライセンス原文は `OFL.txt` に、素材の配布元とSHA-256は配布ZIPの `素材の出典.json` に記載します。 [OFL.txt](OFL.txt)

青磁に関する質問や不具合の報告は、GitHub Issuesで受け付けます。 [Issues](https://github.com/metasta/seiji-fonts/issues)
