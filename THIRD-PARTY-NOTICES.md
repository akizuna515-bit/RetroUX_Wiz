# 第三者のソフトウェア

## この ZIP に含むもの

`runtime\python\` には、RetroUX_Wiz を動かすための第三者のソフトウェアを同梱しています。**これらは RetroUX_Wiz の一部ではなく、`LICENSE` の利用許諾は及びません。** それぞれのライセンスに従います。本文は `licenses\` にあります。

| もの | ライセンス | 本文 | 入手元 |
| --- | --- | --- | --- |
| Python 3.12.10（埋め込み版） | PSF License | `licenses\Python-LICENSE.txt` | https://www.python.org/ |
| PySide6_Essentials・shiboken6 6.11.2（Qt を含む） | LGPL-3.0-only で再配布（配布元の表示は LGPL-3.0-only OR GPL-2.0-only OR GPL-3.0-only） | `licenses\LGPL-3.0.txt`・`licenses\GPL-3.0.txt` | https://pypi.org/project/PySide6-Essentials/6.11.2/ |
| PyYAML 6.0.3（libyaml を含む） | MIT | `licenses\PyYAML-LICENSE.txt`・`licenses\libyaml-License.txt` | https://pypi.org/project/PyYAML/6.0.3/ |
| Qt に含まれる第三者の部品（PCRE2・zlib・FreeType・libpng・HarfBuzz など） | 部品ごとのライセンス | `licenses\Qt-third-party.txt` | Qt のソースに含まれる |
| Python に含まれる第三者の部品（OpenSSL・SQLite・zlib・bzip2・xz・libffi・expat・mpdecimal など） | 部品ごとのライセンス | `licenses\Python-LICENSE.txt`・Python のソース | https://www.python.org/ |
| Microsoft Visual C++ ランタイム（`msvcp140*.dll`・`vcruntime140*.dll`） | Microsoft の再配布の条件。これらのファイルに含まれる Microsoft の表示を変えず、利用者がこれらを単体で再配布しないこと | — | Python・PySide6 の配布物に含まれる |

**PySide6・Qt について**

- ソースコード: PySide6 と shiboken6 は https://code.qt.io/cgit/pyside/pyside-setup.git/ のタグ v6.11.2、Qt は https://code.qt.io/cgit/qt/qtbase.git/ のタグ v6.11.2 から入手できます。
- 改変: ソースもバイナリも改変していません。配布物を小さくするため、使わないファイル（QML・開発用ツール・翻訳・一部のプラグインなど）を外しています。
- 置き換え: `runtime\python\Lib\site-packages\` の `PySide6` と `shiboken6` は、互換のある別の版に置き換えられます。`LICENSE` はこの権利を制限しません。

## この ZIP に含まないもの

利用者が自分で用意します。

| もの | ライセンス |
| --- | --- |
| ファミコン版 Wizardry の ROM | 原作の権利者の著作物 |
| FCEUX 2.6.6 | GPL-2.0-or-later |

## 原作の内容

RetroUX_Wiz は、原作の絵・音・文章、モンスターやアイテムの名前の一覧を含みません。それらは利用者の ROM から実行時に読みます。

ただし、機能の説明のために、一部の呪文の名前とゲームのコマンドの語を、コードと文書に記載しています。

## 色の表

モンスターの絵の色は、利用者の FCEUX の `palettes\FCEUX.pal` から実行時に読みます。ZIP に色の表は入っていません。

## Lua スクリプト

`src\retroux_wiz\lua` の Lua スクリプトは FCEUX の中で動くので、MIT License で提供します（`licenses\MIT-Lua.txt`）。

## RetroUX から移したソース

`src/retroux_wiz` の一部（ジョイパッド・画面の部品・保存の仕組みなど）は、同じ作者の [RetroUX](https://github.com/akizuna515-bit/RetroUX) のソースを元にしています。RetroUX は MIT ライセンスです。元のライセンスの表示を次に写します。

```text
MIT License

Copyright (c) 2026 soichannel3590

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
