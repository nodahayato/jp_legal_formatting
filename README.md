# jp_legal_fromatting

## 使い方

Visual Studio Codeに，拡張機能　[vscode-markdown-pdf](https://github.com/yzane/vscode-markdown-pdf/blob/master/README.ja.md) をインストールして使うことを前提にしたcss設定例です。

### 初期設定

Visual Studio Codeに拡張機能 vscode-markdown-pdf をインストールする。

プロジェクトを作成し，プロジェクト内の .vscode フォルダに csslaw_dev.css をコピーする。

次のアドレスに記載のあるリセットスタイルシートをダウンロードして，
https://code.google.com/archive/p/html5resetcss/downloads
reset.cssの名前で，.vscodeフォルダに保存する。

settings.json の内容をこのプロジェクトのもののように書き換える。
cssの場所を示すパスは各自の環境にあわせて変える。

準備はここまで。

### pdfの作成

プロジェクト内でマークダウンの文書を作成する。

vscode-markdown-pdfでpdfをエクスポートする。
（エクスポートしたいマークダウンファイルの編集画面上で右クリックする。）

### 記法

概ね一般的なマークダウン記法です。

#### 右寄せ

右寄せをcodeで実現しています。右寄せしたい行の冒頭にタブを入れて下さい。

#### 改ページ

改ページをhrで実現しています。改ページしたい場所で --- （半角ハイフンを３つ）入れて下さい。

## 認識している問題点等

* 見出しのナンバリングが半角数字です。cssで実現する方法が見当たらない。
（webシステム等であればいけるけど。）
* 第1→1→(1)までしか対応していない。ア・イ・ウ以下が出力されない。たぶん，拡張機能側の問題。
* 各見出しレベルの下に配置できる本文は１０段落まで。

## バージョン
2020/09/22　とりあえず公開した。
