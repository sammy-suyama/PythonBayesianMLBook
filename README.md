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
| 第4刷まで | p.43 | 下段コードブロック5, 6行目 | # 撹乱項 $\varepsilon$ は平均0の一様分布に従うとする<br>`z_proposal = z_current + step_size * np.random.uniform(-1, 1)` | # 撹乱項 $\varepsilon$ は平均0の正規分布に従うとする<br>`z_proposal = z_current + step_size * np.random.randn()`<br><br>*これに伴い図1.7~図1.13もやや変更あり（本レポジトリのnotebook/1_3_近似推論手法.ipynb参照）。なお、p39に記載の通りランダムウォークMH法では一様分布を利用する場合もあります。 |
| 第4刷まで | p.45 | 下段コードブロック6行目 | `x_proposal = x_current + step_size * np.random.uniform(-1, 1)` | `x_proposal = x_current + step_size * np.random.randn()` |
| 第5刷まで | p.47 | 上段コードブロック5行目 | `az.plot_autocorr(np.array(posterior_large_step[n_burnin:]), ax=ax)` | `az.plot_autocorr(np.array(posterior_large_step), ax=ax)` |
| 第4刷まで | p.47 | 上段コードブロック６行目 | `ax.set_title('step_size = 0.01')` | `ax.set_title('step_size = 10.0')` |
| 第5刷まで | p.47 | 上段コードブロック10行目 | `az.plot_autocorr(np.array(posterior_small_step[n_burnin:]), ax=ax)` | `az.plot_autocorr(np.array(posterior_small_step), ax=ax)` |
| 第4刷まで | p.47 | 上段コードブロック11行目 | `ax.set_title('step_size = 10.0')` | `ax.set_title('step_size = 0.01')` |
| 第4刷まで | p.48 | 図 1.10 | 上段のプロットのタイトル: step_size=0.01<br>中段のプロットのタイトル: step_size=10.0 | 上段のプロットのタイトル: step_size=10.0<br>中段のプロットのタイトル: step_size=0.01 |
