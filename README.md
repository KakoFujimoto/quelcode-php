# データーベースへの接続と探索アルゴリズムに関する問題 

[コードを見る](https://github.com/KakoFujimoto/quelcode-php/blob/master/html/php-pre-challenge3/index.php)

- GETパラメータ[target]から1以上の整数を受け取り、既にデータベースに保存されている数値の羅列から、足してその数になる組み合わせを探しJSON形式で出力します。
- 同数を作る複数の組み合わせがある場合は、全パターンを出力します。
- 組み合わせが存在しない場合は、返却値の例に倣って出力します（出力時の数値や組み合わせの順番は問わないものとする）。

- もし、GETパラメータ[target]値が1以上の整数ではない場合は、HTTP レスポンスステータスコード[400]で返却します。
例) -1,  0, 01, 1.0, 1.1,  number などを受け取った場合

- もしデータベースに接続できない場合は、HTTP レスポンスステータスコード[500]で返却します。

## 動作

- 動作(例)
リクエスト(例)※MAMP環境の場合
http://localhost:10080/php-pre-challenge3/index.php?target=34

- データベースの値(例)
prechallenge3テーブル

|header1|
|:--|
|value|
|17|
|3|
|1|
|13|
|11|
|7|
|19|
|5|
