# FamilyTree

**家系図作成ソフト** — Electron製のデスクトップアプリです。  
縦書き・横書きの家系図ノードで、日本語にも英語にも対応した家系図を直感的に作れます。

![FamilyTree sample](family.png)

---

## 特徴

- **縦書き・横書きの家系図ノード**  
  縦型は名前が縦書き、生年月日・没年月日も縦書きで表示。続柄は名前の右に並びます。  
  横型はコンパクトな横レイアウトで、複数のノードを横に並べた家系図に最適です。

- **サンプル図**  
  ツールバーの「サンプル図」ボタンで、完成した家系図のサンプルを表示します。  
  縦ノードは日本語名・和暦、横ノードは英語名・西暦の例です。  
  表示中はボタンが「サンプルを削除」に変わり、押すとサンプルを開く前の内容に戻ります。  
  サンプルを編集した場合は、「削除して元に戻す」「この図を残す」から選べます。

- **日付の表示切り替え（入力どおり／和暦／西暦）**  
  ツールバーの「日付」で、生年月日・没年月日の表示形式を切り替えられます。初期値は「入力どおり」です。  
  入力した内容は書き換わらず、表示だけが変わります。設定はファイルにも保存されます。  
  読み取れない日付（「不明」「1950年頃」など）は、そのまま表示されます。

- **ノードを枠で囲む**  
  ノードごとに枠線のオン・オフと色を指定できます（初期値はオフ）。

- **サンプル表示（空欄の見本）**  
  ノードごとにオンにすると、空欄の項目に薄い見本の文字を表示します（初期値はオフ）。  
  縦型は日本語名・和暦、横型は英語名・西暦の見本です。

- **フォーク接続（1対多）**  
  1つの親ノードから複数の子ノードへのT字接続線。右クリック→「フォーク接続」で選択・確定するだけ。

- **夫婦線（二重線）**  
  接続線を右クリック→「二重線（夫婦線）に切替」で二重線になります。  
  もう一度右クリックで「一本線に戻す」。

- **中点からのフォーク接続**  
  夫婦線を右クリック→「この線の中点からフォーク接続」で、夫婦の中心から子への接続線が引けます。

- **テキストノード**  
  縦書き・横書きの自由なテキスト枠。枠あり・なし切替可能。

- **背景色の変更**  
  ツールバーの背景カラーピッカーでキャンバスの背景色を自由に変更できます。  
  PNG・SVG・PDF出力時にも反映されます。

- **整列補助線（スナップ線）**  
  ノードをドラッグ中、他のノードの上端・中央・下端・左端・右端に近づくと青い補助線が自動表示されます。揃えたらドロップするだけ。

- **PNG / SVG / PDF 出力**  
  ツールバーから高品質な画像・PDFを出力できます。PDFは図全体が収まる1ページで出力されます。

- **多言語対応**  
  日本語・英語・中国語（簡体・繁体）・韓国語・スペイン語に対応。

- **自動バージョンアップ通知**  
  起動時に最新バージョンを確認し、更新がある場合は案内します。

---

## 操作方法

### ノードの追加
キャンバスを**右クリック** → 「ノードを追加」

### ノードの編集
ノードをクリックして選択 → 右パネルで名前・続柄・生年月日・没年月日・フォント・色・枠・サンプル表示を編集

### ノードを枠で囲む
1. ノードをクリックして選択
2. 右パネルの「枠」で「ノードを枠で囲む」にチェック
3. 隣のカラーピッカーで枠の色を選択

### 日付の表示を切り替える
ツールバーの「日付」で「入力どおり」「和暦」「西暦」を選択します。  
和暦・西暦は、縦ノードでは漢数字（昭和二十五年四月一日）、横ノードでは算用数字（昭和25年4月1日）で表示されます。

### サンプル図を見る
1. ツールバーの「サンプル図」をクリック
2. 確認が終わったら「サンプルを削除」をクリック（編集した場合は確認が出ます）

### 接続線を引く
1. ノードを**右クリック** → 「ここから接続」
2. 接続先のノードをクリック

### フォーク接続（1対多）
1. 親ノードを**右クリック** → 「フォーク接続（1対多）」
2. 子ノードを順にクリックして選択
3. 「確定」ボタンで完了
4. フォーク線を右クリック → 削除

### 夫婦線（二重線）から子供へ接続
1. 夫婦を横並びに配置して接続線を引く
2. 接続線を右クリック → 「二重線（夫婦線）に切替」
3. 同じ線を右クリック → 「この線の中点からフォーク接続」
4. 子ノードを選択して確定

### ファイルの保存・読み込み
- 保存：`Ctrl+S`（`.ft`形式）
- 開く：`Ctrl+O`
- PNG出力：ツールバー「画像出力 (PNG)」
- SVG出力：ツールバー「画像出力 (SVG)」
- PDF出力：ツールバー「画像出力 (PDF)」

---

## 作者

**daigorou-addon**
- [Daigorou-Tools](https://daigorou-addon.github.io/daigorou-tools/)
- Support: [buymeacoffee.com/daigorou](https://buymeacoffee.com/daigorou)


------------------------------------------------------------

# FamilyTree

**Family tree creation software** — An Electron desktop application.
Create family trees intuitively using vertical and horizontal family tree nodes with support for both Japanese and English.

![FamilyTree sample](family.png)

---

## Features

- **Vertical and horizontal family tree nodes**  
  Vertical nodes display names, birth dates, and death dates vertically, while relationships are shown beside the name. Horizontal nodes provide a compact layout suitable for wide family trees.

- **Sample diagram**  
  The "Sample" button in the toolbar shows a completed family tree. The vertical sample uses Japanese names and Japanese-era dates; the horizontal sample uses English names and Gregorian dates.  
  While it is shown, the button changes to "Delete sample", and pressing it restores what you had before. If you edited the sample, you can choose between deleting it and keeping the edited diagram.

- **Date display (as entered / Japanese era / Gregorian)**  
  The "Date" dropdown in the toolbar switches how birth and death dates are displayed. The default is "As entered".  
  What you typed is never rewritten; only the display changes, and the setting is saved with the file. Dates that cannot be read (such as "unknown" or "around 1950") are displayed as typed.

- **Node frame**  
  Turn a frame around a node on or off and choose its color, per node (off by default).

- **Sample text in empty fields**  
  Turn this on per node to show faint sample text in empty fields (off by default). Vertical nodes show Japanese names and Japanese-era dates; horizontal nodes show English names and Gregorian dates.

- **Fork connections (one-to-many)**  
  Connect one parent node to multiple child nodes with a T-shaped branch.

- **Double-line spouse connections**  
  Convert a normal connection into a double-line spouse connection and switch it back at any time.

- **Fork connections from the midpoint**  
  Create child branches directly from the midpoint of a spouse connection.

- **Text nodes**  
  Freely place vertical or horizontal text boxes with or without borders.

- **Background color**  
  Change the canvas background color. The selected color is also reflected when exporting PNG, SVG, or PDF.

- **Alignment guides (snap lines)**  
  Blue alignment guides automatically appear while dragging nodes to help align edges and centers.

- **PNG / SVG / PDF export**  
  Export high-quality images and PDFs directly from the toolbar. The PDF fits the whole diagram on a single page.

- **Multilingual support**  
  Supports Japanese, English, Simplified Chinese, Traditional Chinese, Korean, and Spanish.

- **Automatic update notification**  
  Checks for new versions when the application starts.

---

## How to Use

### Add a node
Right-click the canvas and choose **Add Node**.

### Edit a node
Select a node and edit its name, relationship, birth date, death date, font, colors, frame, and sample text in the right panel.

### Surround a node with a frame
1. Select a node.
2. Check the frame option in the right panel.
3. Pick the frame color with the color picker next to it.

### Switch the date display
Choose "As entered", "Japanese era", or "Gregorian" from the "Date" dropdown in the toolbar.  
Vertical nodes show dates with kanji numerals; horizontal nodes show them with Arabic numerals.

### View the sample diagram
1. Click "Sample" in the toolbar.
2. When you are done, click "Delete sample" (you will be asked to confirm if you edited it).

### Create a connection
1. Right-click a node and choose **Connect from here**.
2. Click the destination node.

### Fork connection (one-to-many)
1. Right-click the parent node.
2. Choose **Fork Connection (One-to-Many)**.
3. Select child nodes.
4. Click **Confirm**.

### Connect children from a spouse line
1. Create a spouse connection.
2. Convert it to a double line.
3. Right-click the line and create a fork connection from its midpoint.
4. Select the child nodes.

### Save, open, and export
- Save: `Ctrl+S` (`.ft` format)
- Open: `Ctrl+O`
- Export: PNG / SVG / PDF buttons in the toolbar

---

## Author

**daigorou-addon**
- [Daigorou-Tools](https://daigorou-addon.github.io/daigorou-tools/)
- Support: https://buymeacoffee.com/daigorou
