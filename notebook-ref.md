# Notebook補足情報

## 動作確認済み環境情報
2019年4月時点で、Notebookの動作確認は以下の環境で行っています。

- Anaconda 2018.12 for Windows
- Anaconda 2018.12 for Mac
- Watson Studio
- Google Colaboratory

Google Colaboratoryで利用するための手順に関しては、qiitaに記事 [書籍「ディープラーニングの数学」のNotebookをGoogle Colaboratoryで動かす](https://qiita.com/makaishi2/items/8a7f530ad9b18b1f0b61) を記載しましたので、こちらを参照されて下さい。

### Windows / MAC
Anaconda 2018.12 for Windows(Mac) Installer  
ライブラリ別のバージョンは以下の通りとなっています。  
(2019-03時点)

```
python 3.7.1
numpy 1.15.4
pandas 0.23.4
matplotlib 3.0.2
scipy 1.1.0
scikit-learn 0.20.1
Jupyter 4.4.0
```

### Watson Studio
ライブラリ別のバージョンは以下の通りとなっています。  
(2019-09時点)

```
python 3.6.8
numpy 1.15.4
pandas 0.24.1
matplotlib 3.0.2
scipy 1.2.0
scikit-learn 0.20.3
Jupyter 4.4.0
```

### Google Colaboratory
ライブラリ別のバージョンは以下の通りとなっています。  
(2019-05時点)

```
python 3.6.7
numpy 1.16.3
pandas 0.24.2
matplotlib 3.0.3
scipy 1.2.1
scikit-learn 0.20.3
Jupyter 4.4.0
```


## 11章のNotebookを動かすための追加手順
　本書p.309に記載したとおり、Anacondaデフォルト環境にKerasのライブラリは導入されていないため11章付属のサンプルコードは稼働しません（Watson Studio/Google Colaboratoryでは稼働します）。  
　著者が確認した手順を以下のリンク先にアップしておきましたので参考とされて下さい。

qiita記事  
[Windows/MACのJupyter NotebookからKerasが使えるようにする](https://qiita.com/makaishi2/items/f8512c0c4828ddea51ca)

## Notebookプログラムの制限事項と対応策
2019年3月28日時点で判明しているNotebookプログラムの制限事項と対応策は次の通りです。

|章|プラットフォーム|内容|対策|
|---|---|---|---|
|10|Watson Studio|学習にかなりの時間を要します。|学習自体はできるので結果が戻るまで待っていてください。|
|11|Mac|環境によりグラフ描画ができない場合があります。|回避策用のコードを含めたnotbookファイルch11-keras-mac.ipynbを用意しました。必ずこちらを利用して、最初のセルのコードも実行するようにしてください。|

[メインページに戻る](./README.md)