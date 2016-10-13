# Chainerの基本：機械学習

ニューラルネットワークを含んだ多くの機械学習における学習タスクは最適なパラメータを探す問題です。

そして，最適なパラメータは目的関数の最小化（最大化）問題を解くことで自動的に得られます。

一般に何かを学習させたいという場合は次のステップからなります。

1) 学習対象のモデルを定義する

Chainerの場合，Function, Link, Chainを組み合わせて入力から出力を求める関数を定義することに対応します。

2) 目的関数 $L(F(\theta))$ を定義する

Chainerの場合，Classifierや損失関数（例：F.soft_cross_entropyや，F.mean_squared_error）を使うことに対応します。

3) 目的関数を最小化するような$\theta$を最適化問題を解くことで得る

Chainerの場合，Optimizerを使って学習させることに対応します。

これらを順に紹介していきます。




