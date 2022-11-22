# SpeechRecognitionGoogle

`.wav` データの文字起こし

## wip

取り急ぎ実装はできたが、適当なコピペ貼り付けなので整理する

[pythonで長い音声・動画からの文字起こしを実装する | ハムレット型エンジニアのカンニングノート](https://www.hamlet-engineer.com/posts/mojiokoshi_long.html)

[【Python】文字お越しのサンプル SpeechRecognitionを利用 | プログラミングで人生が楽になりました](https://posipochi.com/2021/04/05/mojiokoshi/)


### todo

- 全般的なこと
  - 変数名
  - `open` `close` を`with` でまとめる
  - `pathlib`
- speechRecognition なこと
  - よきような書き方

## setup

### pip

``` terminal
python -m pip install SpeechRecognition
python -m pip install numpy
```

scipy 不要かも

``` terminal
% >python -m pip list
Package           Version
----------------- -------
numpy             1.23.5
pip               22.3.1
setuptools        60.2.0
SpeechRecognition 3.8.1
wheel             0.37.1

```

### 手作業（になっているもの）

ディレクトリ作成

``` .txt
audio/
output/
    cut_wav/
```