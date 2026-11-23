# Seiji / 青磁

[日本語](README.md)

Seiji is a set of Japanese typefaces whose kanji forms follow the selection criteria of I.Ming Seiji. Seiji Mincho, Seiji Gothic, and Seiji Maru Gothic each come in Regular and Bold.

[Download the fonts](https://github.com/metasta/seiji-fonts/releases)

![Horizontal specimen comparing Regular and Bold in Seiji Mincho, Seiji Gothic, and Seiji Maru Gothic. The sample describes waiting for a friend at a station at dusk, with 駅 shown in the form 驛.](seiji-specimen.png)

## Installation

### Word and other apps

Extract the release ZIP and install the OTF files for your chosen typeface. Install both files if you need both weights. Choose the typeface from your app’s font menu.

| English menu name | Japanese menu name |
| --- | --- |
| Seiji Mincho | 青磁明朝 |
| Seiji Gothic | 青磁ゴシック |
| Seiji Maru Gothic | 青磁丸ゴシック |

### Web browsers

Chrome and Firefox let you select an installed font as the browser default. This applies where the page relies on browser defaults. Site-specific font choices may still apply. [Chrome settings](https://support.google.com/chrome/answer/96810?hl=en) · [Firefox settings](https://support.mozilla.org/en-US/kb/change-fonts-and-colors-websites-use)

Safari on macOS offers a user style sheet setting under Advanced. Its settings do not include a default font picker. The Seiji release ZIP includes CSS for Japanese page content. The guide explains how to apply it and when site fonts can still appear. [Safari setup and scope (Japanese)](docs/safari.md)

## Character coverage

The 0.300 preview includes 1,026 educational kanji and 400 additional jōyō kanji, for a total of 1,426 across all six fonts. The release ZIP includes the complete list in `収録漢字.txt`.

## Contextual forms and literal glyphs

辯, 辨, and 瓣 are distinct kanji that share the form 弁 in modern Japanese. When the OpenType `calt` feature is enabled, 弁論, 弁別, and 花弁 appear as 辯論, 辨別, and 花瓣, respectively.

If a line break separates the characters needed by a rule, some apps may skip that rule. As a result, even automatic wrapping due to changes in window width or text size can affect the displayed form.

To display 灯 in the sense of “lamplight,” or 余 or 予 as first-person pronouns, enter `灯󠄀`, `余󠄀`, or `予󠄀` in an app that supports ideographic variation sequences (IVS). In each sequence, U+E0100 follows the kanji. Seiji 0.300 provides this option for the 13 sequences listed in the reference table. [Contextual rules and IVS reference (Japanese)](docs/contextual-forms.md)

## Technical documentation

These documents are in Japanese.

- [Kanji and kana coverage](docs/coverage.md)
- [Kanji selection and Seiji’s glyph design](docs/glyph-selection.md)
- [Contextual forms and ideographic variation sequences](docs/contextual-forms.md)
- [Safari setup and style sheet scope](docs/safari.md)
- [Known display limitations](docs/known-issues.md)

## License and sources

Seiji is distributed under the SIL Open Font License 1.1, including the fonts embedded in the Safari CSS. See `OFL.txt` for copyright notices and the license text. The release ZIP lists source URLs and SHA-256 hashes in `素材の出典.json`. [OFL.txt](OFL.txt)

Questions and bug reports are welcome on GitHub. [Issues](https://github.com/metasta/seiji-fonts/issues)
