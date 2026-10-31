# 第三者のソフトウェア

## この ZIP に含まれないもの

次のものは ZIP に入っていません。利用者が自分で用意するか、`uv sync` が公式の配布元から入れます。それぞれのライセンスに従ってください。

| もの | ライセンス | 入手 |
| --- | --- | --- |
| ファミコン版 Wizardry の ROM | 原作の権利者の著作物 | 自分が正当に持っているもの |
| FCEUX 2.6.6 | GPL-2.0-or-later | 利用者が入手 |
| uv | uv の配布物の表示に従ってください | 利用者が入手 |
| Python 3.12 | PSF License | uv が入手 |
| hatchling とその依存 | それぞれの配布物の表示に従ってください | `uv sync` がビルドの道具として PyPI から入手。実行には使わない |
| PySide6・PySide6_Essentials・PySide6_Addons・shiboken6 6.11.2 | LGPL-3.0-only OR GPL-2.0-only OR GPL-3.0-only | `uv sync` が PyPI から入手 |
| PyYAML 6.0.3 | MIT | `uv sync` が PyPI から入手 |

## 原作の内容

RetroUX_Wiz は、原作の絵・音・文章、モンスターやアイテムの名前の一覧を含みません。それらは利用者の ROM から実行時に読みます。

ただし、機能の説明のために、一部の呪文の名前とゲームのコマンドの語を、コードと文書に記載しています。

## 色の表

モンスターの絵の色は、利用者の FCEUX の `palettes\FCEUX.pal` から実行時に読みます。ZIP に色の表は入っていません。

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
