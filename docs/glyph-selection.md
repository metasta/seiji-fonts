# 字形の選定と調整

青磁は、一点明朝正字 v1.1を漢字の字形選びの基準とします。字の成り立ちと日本語での用法を確かめ、明朝・ゴシック・丸ゴシックそれぞれの素材から字形を選びます。収録する漢字は、3書体のRegularとBoldの全6本で確認します。 [一点明朝正字の字形選定基準](https://github.com/epistularum/kanji-restoration#正字-criteria)

## 書体間で共通にする形

字を構成する部分の区別を保った上で、部分同士の接触や分離に選択の余地がある場合は、上下の構成を読み取りやすい形を選ぶことがあります。一点明朝正字が参照する『傳承字形部件檢校表』の表三では、構成する部分が混同されない範囲の接触や分離を、設計上の差の例に含めます。 [『傳承字形部件檢校表』1.37（本文111〜113頁）](https://github.com/ichitenfont/inheritedglyphs/blob/master/component_of_recom_inherited_glyphs-1.37.pdf)

青磁 0.200では、「走」と「起」に含まれる「走」の両方に、上部と下部が分かれた形を採用しました。この選択は6本で共通です。

## 書体ごとの素材

素材ごとの配布元、著作権表示、SHA-256は、配布ZIPの `素材の出典.json` で確認できます。 [青磁 0.200の配布ZIP](https://github.com/metasta/seiji-fonts/releases/tag/v0.200)

| 素材 | 青磁での役割 |
| --- | --- |
| [しっぽり明朝](https://github.com/fontdasu/ShipporiMincho) | 青磁明朝のかな・約物・欧文と組版の基本設定 |
| [源流明朝](https://github.com/ButTaiwan/genryu-font) | 青磁明朝の漢字素材 |
| [源石ゴシック](https://github.com/ButTaiwan/genseki-font) | 青磁ゴシックの基本設定と漢字素材 |
| [源泉丸ゴシック](https://github.com/ButTaiwan/gensen-font) | 青磁丸ゴシックの基本設定と漢字素材 |
| [源ノ明朝](https://github.com/adobe-fonts/source-han-serif)・[源ノ角ゴシック](https://github.com/adobe-fonts/source-han-sans) | 漢字の形の再生成と、各書体で共通に参照する原稿 |
| [さらら明朝](https://www.akenotsuki.com/eyeben/fonts/sarara.html)・[霧ゴシック](https://www.akenotsuki.com/eyeben/fonts/kirigo.html) | ア行エ・や行えの素材 |
