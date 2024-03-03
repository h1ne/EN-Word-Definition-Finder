# English Word Definition Finder

<img src="https://img.shields.io/badge/-BeautifulSoup-3776AB.svg?logo=python&style=social">

## 内容
本プログラムはPythonライブラリであるBeautifulSoupにより英単語の意味を自動で取得するプログラムです。
単語の意味は、[ロングマン現代英英辞典](https://www.ldoceonline.com/)より自動で取得され、指定のExcelファイルへ書き出される仕組みになっております。

ファイル構成
```
README.md                               本説明ファイル
definition-finder.py                    プログラム
definition-finder2.py                   リファクタ済プログラム
```

---

## 環境構築
本プログラムを実行するには、Pythonが実行できる環境の他にそのライブラリが使える環境が必要です。
Pythonの実行環境は整っている状態を想定して環境構築を行います。pipを用いてライブラリをインストールします。

```
pip install requests beautifulsoup4 openpyxl
```

---

## 使用方法
初めに、以下の画像のようにExcelファイルの１カラムに調べたい単語をリストアップします。
<img width="529" alt="image1" src="https://github.com/h1ne/wordwhiz/assets/130957043/20451039-84f7-4e99-bc21-8f05255d2e09">

次に、作成したExcelファイルをプログラムと同じ階層のディレクトリに配置します。この時、プログラム内の以下の部分の`FILE NAME`を**拡張子を除いた**Excelのファイル名に変更します。

```
# File info
FileName = "FILE NAME" # Set file name
Extension = ".xlsx" # Set Extension
```

ここまでの設定が終わったらPythonプログラムを実行するとExcelファイル内の２カラムに意味が書き込まれます。

※ここで上手く実行できない場合は、Excelのファイル名が原因になっている可能性があります。

---

## 免責事項
このプログラムの使用により生じたいかなる障害、損害、不具合等について、私と私の関係者及びいかなる団体・組織とも、一切の責任を負いません。各自の責任にてご自由にお使いください。