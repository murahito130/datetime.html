# datatime.html

`datatime.html` は、現在の日付と時刻をシンプルに表示するウェブアプリケーションです。OBSなどの配信ツールでのオーバーレイ表示や、デスクトップのカスタマイズなど、様々な用途で活用できます。

## 使い方

### オンラインで利用する

GitHub Pagesで公開されている以下のURLから、直接アプリを利用できます。

[`https://murahito130.github.io/datetime.html`](https://murahito130.github.io/datetime.html)

URLパラメータを追加することで、表示をカスタマイズできます。

### ダウンロードして利用する

1. このリポジトリをクローンまたはダウンロードします。

2. ダウンロードしたフォルダ内の `index.html` ファイルをウェブブラウザで開きます。

## カスタマイズ

URLパラメータを使用することで、表示される日付と時刻の背景色、文字色、配置、**文字サイズ、全体のサイズ**を柔軟にカスタマイズできます。また、1分間の進捗を示すプログレスバーの表示を切り替えることも可能です。

### 利用可能なパラメータ

* **`bgColor`**: ページ全体の背景色。

  * デフォルト値: `transparent`

  * 例: `bgColor=000000` (黒), `bgColor=red`

* **`containerBgColor`**: メインコンテナの背景色。

  * デフォルト値: `FFFFFF` (白)

  * 例: `containerBgColor=FFFFFF` (白)

* **`dateBgColor`**: 日付表示部分の背景色。

  * デフォルト値: `E2BEE6`

  * 例: `dateBgColor=E2BEE6`

* **`dateTextColor`**: 日付表示部分の文字色。

  * デフォルト値: `6D2A84`

  * 例: `dateTextColor=6D2A84`

* **`timeBgColor`**: 時刻表示部分の背景色。

  * デフォルト値: `CD93D7`

  * 例: `timeBgColor=CD93D7`

* **`timeTextColor`**: 時刻表示部分の文字色。

  * デフォルト値: `48148A`

  * 例: `timeTextColor=48148A`

* **`dateAlign`**: 日付表示のテキストアラインメント。

  * デフォルト値: `left`

  * 値: `left`, `center`, `right`

* **`dateFontSize`**: 日付表示部分の文字サイズ。

  * デフォルト値: `0.85em`

  * 例: `dateFontSize=1.5em`, `dateFontSize=24px`

* **`timeFontSize`**: 時刻表示部分の文字サイズ。

  * デフォルト値: `3.5em`

  * 例: `timeFontSize=4em`, `timeFontSize=72px`

* **`scale`**: 全体の表示サイズ（拡大・縮小）。

  * デフォルト値: `1.0`

  * 例: `scale=0.8` (80%に縮小), `scale=1.2` (120%に拡大)

* **`fontFamily`**: 表示フォント。

  * デフォルト値: `Inter`

  * 例: `fontFamily=Arial`, `fontFamily="Noto Sans JP"` (スペースを含む場合は引用符で囲む)

* **`showProgressBar`**: 1分間の進捗を示すプログレスバーの表示・非表示。

  * デフォルト値: `false` (非表示)

  * 値: `true`, `false`

**色の指定について:**
色の値は、`RRGGBB`形式の16進数コード（例: `FF0000`）またはCSSのカラーネーム（例: `red`）で指定できます。

### URLパラメータの例

以下のURLの例は、`https://murahito130.github.io/datetime.html` をベースにしています。

1. **デフォルト設定 (パラメータなし):**
   https://murahito130.github.io/datetime.html

   **表示例:**
   
   ![デフォルト表示](example1.png)

2. **プログレスバーを有効にして表示:**
   https://murahito130.github.io/datetime.html?showProgressBar=true

   **表示例:**
   
   （プログレスバーが時間表示の下部に表示されます）

3. **背景色を黒、メインコンテナの背景色を白に設定:**
   https://murahito130.github.io/datetime.html?bgColor=000000&containerBgColor=FFFFFF

   **表示例:**
   
   ![背景色黒、コンテナ白](example2.png)

4. **日付表示の背景を赤、文字を白に、時刻表示の背景を青、文字を黄色に設定:**
   https://murahito130.github.io/datetime.html?dateBgColor=FF0000&dateTextColor=FFFFFF&timeBgColor=0000FF&timeTextColor=FFFF00

   **表示例:**
   
   ![日付赤白、時刻青黄](example3.png)

5. **日付を中央揃えに設定:**
   https://murahito130.github.io/datetime.html?dateAlign=center

   **表示例:**
   
   ![日付を中央揃え](example4.png)

6. **すべてのパラメータを組み合わせて設定:**
   https://murahito130.github.io/datetime.html?bgColor=333333&containerBgColor=E0E0E0&dateBgColor=FFD700&dateTextColor=8B4513&timeBgColor=ADD8E6&timeTextColor=000080&dateAlign=right

   **表示例:**
   
   ![全パラメータ組み合わせ](example5.png)
