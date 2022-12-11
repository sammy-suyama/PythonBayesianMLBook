# PythonBayesianMLBook
「Pythonではじめるベイズ機械学習入門」のサポートページです。
本で紹介されているソースコードや正誤表を掲載していく予定です。

## notebookの実行環境
2022年5月現在、Google Colaboratoryで実行するのが一番簡単です。 各notebookの下記アイコンをクリックするだけで開けます。 
![colab-badge](https://colab.research.google.com/assets/colab-badge.svg)

今後、Colaboratoryのライブラリのバージョン変更などで動かなくなった場合、書籍に記載のバージョンをインストールして実行してください。requirements.txtも用意してあります。 

## 正誤表

| 版 | ページ | 該当箇所 | 誤 | 正 |
| --- | --- | --- | --- | --- |
| 例 | p.47 | 上段コードブロック６行目 | ax.set_title('step_size = 0.01') | ax.set_title('step_size = 10.0') |
| 例 | p.47 | 上段コードブロック11行目 | ax.set_title('step_size = 10.0') | ax.set_title('step_size = 0.01') |
| 例 | p.48 | 図 1.10 | 上段のプロットのタイトル: step_size=0.01, 中段のプロットのタイトル： step_size=10.0 | 上段のプロットのタイトル: step_size=10.0, 中段のプロットのタイトル： step_size=0.01 |
