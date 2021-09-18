Day１ 強化学習の位置づけを知る
===

###### tags: `Pyhtonで学ぶ 強化学習[改定第2版] 入門から実践まで`


# 1.1 強化学習とさまざまなキーワードの関係

* 教師なし学習
    * いまいち教師なし学習がなんなのか理解してない

* 強化学習
    * データ
    * 環境
    * 行動
    * 報酬

# 1.2 強化学習のメリット・デメリット

* 教師あり学習だとその場その場の選択での評価になる
* 強化学習だとある期間内など一定の幅を持った最適な選択を評価できる
* 強化学習で学習させるもの
    * 行動の評価方法
    * 評価に基づく行動の選択

* メリット・デメリット
    * メリット： 各行動に対する評価が難しい問題でも溶ける可能性がある
    * デメリット:獲得される行動が制御できない

# 1.3 強化学習における問題設定：Markov Decision Process

 $$ a = \pi(s_t) $$
 $$ r = R(s. s^{'}) $$

# code