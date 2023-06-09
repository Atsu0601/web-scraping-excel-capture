# capture-web-scraping
Excel ベースの URL リストの情報から自動でサイトを辿り、キャプチャ（PC/SP）を保存する機能です。  
同時に保存したキャプチャは、新しく生成した Excel に添付されます。

## Dependency
動作確認済み環境  
macOS ma1 10.12.6  
Python 3.11.0 

## Setup
### Python
https://www.python.org/downloads/  
3系の最新バージョンをインストール

ターミナルを開いて、以下のコマンドを実行。
```
$ python --version
```
バージョンが表示されたらOK。

### pip
ターミナルを開いて、以下のコマンドを実行。
```
$ easy_insatll pip
```

### selenium
ターミナルを開いて、以下のコマンドを実行。
```
$ pip install selenium
```

### Chrome Driver
ターミナルを開いて、以下のコマンドを実行。
```
$ brew cask install chromedriver
```

### xlrd
xlrd　でエラーが出た場合は、下記のコマンドを実行
xlrd　はxlsxの拡張子を最新バージョンはサポートしてないため。
```
pip3 install xlrd==1.2.0
```

### Python ライブラリインストール
ターミナルを開いて「requirements.txt」と同じディレクトリにいる状態で、以下のコマンドを実行。
```
$ pip install -r requirements.txt
```

## Usage
### url.xlsx
必要な情報を記入。  
A列：ID  
B列：タイトル  
C列：URL  

### 実行
ターミナルを開いて、以下のコマンドを実行。
```
$ python capture.py
```

## Licence
This software is released under the MIT License, see LICENSE.

## Author
[Shuny125](https://github.com/Shuny125)

## References
http://xlsxwriter.readthedocs.io/
