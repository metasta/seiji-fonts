# 字形の選定と調整

正字とされる字形は書体によって異なることがあります。青磁では、明朝・ゴシック・丸ゴシックを同じ文書で併用することを想定し、3書体とも[一点明朝正字の字形選定基準](https://github.com/epistularum/kanji-restoration#正字-criteria) に沿って漢字の字形を選びます。

## 書体間で共通にする形

一点明朝正字が参照する『傳承字形部件檢校表』では、構成する部分が混同されない範囲の接触や分離は正字基準に影響せず、書体設計上の差に含まれます。青磁でも、書体によって部品間の接触/分離に差がある字については、基本的に各素材の字形をそのまま採用しました。ただし、接触/分離の差により筆画の構成が把握しにくくなる一部の字については、他の部品との混同はなくても筆画構成を明確にする調整を施しました。青磁 0.200における「走」や「起」での「土」・「龰」の分離はその一例です。

このため青磁差であり、に含めます。 [『傳承字形部件檢校表』1.37（本文111〜113頁）](https://github.com/ichitenfont/inheritedglyphs/blob/master/component_of_recom_inherited_glyphs-1.37.pdf)

## 書体ごとの素材

素材ごとの配布元、著作権表示、SHA-256は、配布ZIPの `素材の出典.json` で確認できます。 [青磁 0.300の配布ZIP](https://github.com/metasta/seiji-fonts/releases/tag/v0.300)

| 素材 | 青磁での役割 |
| --- | --- |
| [しっぽり明朝](https://github.com/fontdasu/ShipporiMincho) | 青磁明朝のかな・約物・欧文と組版の基本設定 |
| [源流明朝](https://github.com/ButTaiwan/genryu-font) | 青磁明朝の漢字素材 |
| [源石ゴシック](https://github.com/ButTaiwan/genseki-font) | 青磁ゴシックの基本設定と漢字素材 |
| [源泉丸ゴシック](https://github.com/ButTaiwan/gensen-font) | 青磁丸ゴシックの基本設定と漢字素材 |
| [源ノ明朝](https://github.com/adobe-fonts/source-han-serif)・[源ノ角ゴシック](https://github.com/adobe-fonts/source-han-sans) | 漢字の形の再生成と、各書体で共通に参照する原稿 |
| [さらら明朝](https://www.akenotsuki.com/eyeben/fonts/sarara.html)・[霧ゴシック](https://www.akenotsuki.com/eyeben/fonts/kirigo.html) | ア行エ・や行えの素材 |
