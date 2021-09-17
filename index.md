「Pyhtonで学ぶ 強化学習[改定第2版] 入門から実践まで」インデックスページ
===

###### tags: `Pyhtonで学ぶ 強化学習[改定第2版] 入門から実践まで`

# 目次
- [Day1 強化学習の位置づけを知る](https://hackmd.io/BGivs-T-RMqBP_f9ppF4lQ)

# 進め方
テキストは当日読めばOK

区切りのいい部分まで20分くらい時間をとって、読む
↓
分からない部分を共有する

コード部分も時間をとって、写経

次回は 9/18 土曜日 15:00 から

# 環境構築
**サポートコンテンツ** 内の環境構築を実施
Anaconda/miniconda で仮想環境を作成してライブラリをダウンロード

## Pythonの仮想環境のはなし
pip が古いのでアップデートしておくと安心

### 仮想環境作成
仮想環境の作成
```shell=
conda create -n 環境名　python=X.X
```
* pythonのバージョンによっては他のパッケージとモメる

miniconda:

自分のユーザー名/.conda/envs/rl-book/ の中に入っている(kazumichi)

Anaconda:

自分のユーザー名/anaconda3/envs/rl-book/ の中に入っている(とよだ)

* 管理者権限でしかファイル作成できないときは，プロンプトを管理者権限で立ち上げる

仮想環境の削除:
``` shell=
conda remove -n 環境名 --all
```
仮想環境に入る:
```shell=
conda activate 環境名
```
仮想環境を抜ける:
```shell=
conda deactivate
```


### 仮想環境とパス
(rl-book) 内のパスも，ある程度は，windowsのパスを継承しているらしい，でも
python関係はenvs/rl-book
git は C:\Program Files\Git\cmd

(rl-book) でgitが通らない場合は，windowsのpathにgit を通しておけば，
(rl-book) にpathがコピーされてうまくうごく

### 仮想環境のエクスポートとインポート

#### 仮想環境のエクスポート

仮想環境の情報をエクスポートするには以下のコマンドをAnaconda/miniconda prompt上で実行

``` shell=
    $ conda env export > [出力ファイル名]
```

具体例：YAML形式でエクスポート

``` shell=
    $ conda env export > environment.yml
```

#### 仮想環境のインポート

YAMLファイルなどから設定を取り込んで仮想環境を構築する

``` shell=
$ conda env create --file [ファイル名]
```