## ちょるボット　README

>  ちょるボットは，自己満足のためのボットです．なのでバグや計算間違いなどのプログラムのミス，返信が帰ってこなかったり等の設備不良によって生じた，いかなる損失・損害・トラブルに対しても責任を負うことはしません．悪しからず．

#### コマンド
---

* [list](#List)
* [help](#Help)
* [destination](#Destination)
* [problem](#Problem)
* [function](#Function)
    * 整数論（パート１）  
        * pow　（べき乗）
        * factorial　（階乗）
        * gcd　（最大公約数）
        * lcm　（最小公約数）
    * 整数論（パート２）
        * eea （拡張ユークリッドの互除法）
        * mod_inv　（合同式の逆元）
        * totient　（オイラー関数・トゥーシェント関数）
        * chinese　（中国人剰余の定理が成り立つ連立合同式の解）
    * 組み合わせ・順列
        * perm　（重複なし順列）
        * perm_rep　（重複あり順列）
        * comb　（重複なし組み合わせ）
        * comb_rep　（重複あり組み合わせ）
    * お遊び（パート１）
        * egyptian_fraction　（エジプト分数展開）
        * rand　（ランダムな数が帰ってくる）

[List]: https://github.com/mk95kagakushi/mk95_bot/blob/master/README.md#List
[Help]: https://github.com/mk95kagakushi/mk95_bot/blob/master/README.md#Help
[Function]: https://github.com/mk95kagakushi/mk95_bot/blob/master/README.md#Function
[Destination]: https://github.com/mk95kagakushi/mk95_bot/blob/master/README.md#Destination
[Problem]: https://github.com/mk95kagakushi/mk95_bot/blob/master/README.md#Problem

-------


### <a name ="List"> list コマンド
> @choll_bot list   

とリプを送ることで，実装されているコマンド・関数のリストが書かれたURLが帰ってきます．

＜未実装＞

> @choll_bot list DM  

[ DM ]とオプションをつけることで，ダイレクトメッセージにリストを送られてきます．

＜未実装＞

> @choll_bot list random

[ random ]とオプションをつけることで，ランダムに関数を３つ教えてくれます．

---

### <a name ="Help"> help コマンド
> @choll_bot help 関数名

とリプを送ることで，指定した関数のフォーマットが帰ってきます．関数名の部分はlistを参照してください

＜未実装＞

> @choll_bot help English

[ English ]とオプションをつけることで，英語で書かれたhelpが返ってきます．

---

### <a name ="Destination"> destination コマンド

＜未実装＞

> @choll_bot destination @ユーザーネーム

とリプを送ることで，指定したユーザーにコマンドの実行結果を送ります．

---

### <a name ="Problem"> problem コマンド

＜未実装＞

> @choll_bot problem 問題番号 解答

とリプを送ることで，指定した番号の正誤判定ができます．

---

### <a name ="Function"> function コマンド

> また今度，全体的に加筆します．  
> 間違っていたり，変なところ，改善案はダイレクトメッセージに送ってください．
> 変なフォーマットのリプは，なるべく送らないでください．
#### 整数論（パート１）

---

####pow
> @choll_bot pow x n

x:整数  
n:整数  
とリプを送る事で，xのn乗が返ってきます．

---

####factorial
> @choll_bot factorial x

x:整数  
とリプを送る事で，x! (xの階乗)が返ってきます．

---

####gcd
> @choll_bot gcd x y

x:整数  
y:整数  
とリプを送る事で，xとyの最大公約数が返ってきます．

---

####lcm
> @choll_bot lcm x y

x:整数  
y:整数  
とリプを送る事で，xとyの最小公約数が返ってきます．

---

#### 整数論（パート２）

####eea
> @choll_bot eea x y

x:整数  
y:整数  
とリプを送る事で，a*x+b*y=c を満たす
a x b y c が返ってきます．

---

####mod_inv
> @choll_bot mod_inv a m

a:整数  
m:整数  
とリプを送る事で，a*x ≡ 1 (mod m) を満たす xが返ってきます． mを法としてaの逆元を求めています．

---

####totient
> @choll_bot totient x

x:整数  
とリプを送る事で，オイラー関数・トゥーシェント関数・φ(x)が返ってきます．  
この関数は，xと互いに素なx未満の自然数の個数を求めています．

---

####chinese
> @choll_bot chinese n a1 m1 a2 m2 ... an mn

n:整数  
ai:整数  
mi:整数  
とリプを送る事で  
a1 ≡ x (mod m1)  
a2 ≡ x (mod m2)  
...  
an ≡ x (mod mn)  
を満たす x が帰ってきます．

---

#### 組み合わせ・順列

####perm
> @choll_bot perm n r

n:整数  
r:整数  
とリプを送る事で，nPr 重複なし順列の値が返ってきます．

---

####perm_rep
> @choll_bot perm_rep n r

n:整数  
r:整数  
とリプを送る事で，nΠr 重複あり順列の値が返ってきます．

---

####comb
> @choll_bot perm n r

n:整数  
r:整数  
とリプを送る事で，nCr 重複なし組み合わせの値が返ってきます．

---

####comb_rep
> @choll_bot comb_rep n r

n:整数  
r:整数  
とリプを送る事で，nHr 重複あり順列の値が返ってきます．

---

#### お遊び（パート１）

####egyptian_fraction
> @choll_bot egyptian_fraction a b

a:整数  
b:整数  
とリプを送る事で，a/b = 1/n1 + 1/n2 + ... + 1/nk となる ni　が返ってきます．  
この分解は複数の答えがありますが，そのうちの１種類が返ってきます．

---

＜未実装＞

####rand
> @choll_bot rand a b

a:整数  
b:整数  
とリプを送る事で，a以上 b以下のランダムな数値が１つ返ってきます．

---
