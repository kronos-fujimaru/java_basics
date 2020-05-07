# Java入門 演習問題

C:￥itc￥java_basicフォルダを作成し、各演習のJavaファイルを作成、実行しなさい。

<br>

## 演習1（ex01.java）
変数aと変数bに格納されている値を入れ替え、値を表示しなさい。

```java
class ex01 {
    public static void main(String[] args) {
        int a = 10;
        int b = 20;

        ???
    }
}
```

**出力結果**

```
変数a = 20
変数b = 10
```

<br>

## 演習2（ex02.java）
実行時引数で点数（整数値）を入力し、80以上は「優良」、50点以上80点未満は「良」、30点以上50点未満は「可」、30点未満は「不可」を表示しなさい。

> Javaでは、mainメソッドの引数のargs変数（配列）に実行時引数の値が格納される。また、String型をint型に変換するには Integer.parseIntメソッドを用いる。

```java
class ex02 {
    public static void main(String[] args) {
        System.out.println("点数：" + args[0] + "点");
        int score = Integer.parseInt(args[0]);

        ???
    }
}
```

**出力結果**<br>※実行時引数に80を入力した場合

```
点数：80点
優良
```

<br>

## 演習3（ex03.java）
実行時引数で数値を入力し、数値が3の倍数の時は "3の倍数"、数値が5の倍数の時は "5の倍数"、数値が7の倍数の時は "7の倍数"、数値が11の倍数の時は "11の倍数"と表示しなさい。例えば、入力された数値が231の場合は、"3の倍数"と"7の倍数"と"11の倍数"を表示する。

**出力結果**<br>※実行時引数に231を入力した場合

```
3の倍数
7の倍数
11の倍数
```

<br>

## 演習4（ex04.java）
実行時引数で年齢と学生証（0:無、1:有）の2つの値を入力し、以下のように金額を表示しなさい。

- 20歳以上は、1800円
- 65歳以上は、1500円
- 20歳未満または学生証を持っている人は、1200円

**出力結果**<br>※実行時引数で25、1（年齢25歳、学生証有）を指定した場合

```
1200円
```

<br>

## 演習5（ex05.java）
1から100までの数値を順に足した結果を表示しなさい。

**出力結果**

```
1
3
6
10
15
21
28
36
45
55
...（中略）
5050
```

<br>

## 演習6（ex06.java）
1から100の間の偶数値の総和を表示しなさい。

**出力結果**

```
合計：2550
```

<br>

## 演習7（ex07.java）
配列に格納されている数値のうち最大値を表示しなさい。

```java
int[] scores = {80, 72, 64, 81, 90, 56, 79, 92, 43, 78};
```

**出力結果**

```
最大：92
```

<br>

## 演習8（ex08.java）
配列に格納されている数値の絶対値の総和を表示しなさい。

```java
int[] values = {50, 23, -64, 38, -10, 13, 41, -35, -5, 26};
```

**出力結果**

```
合計：305
```

<br>

## 演習9（ex9.java）
実行時引数で複数の数値を入力させ、総和を表示しなさい。

**出力結果**<br>※実行時引数に10,20,30の3つの数値を入力した場合

```
合計：60
```

<br>

## 演習10（ex10.java）
"★"を3行5列表示しなさい。ただし、以下のステートメントをそれぞれ1回だけ用いることとする。

- System.out.print("★");
- System.out.println();

**出力結果**

<img src="img/ex10.png" width="300">

<br><br>

## 演習11（ex11.java）
"★"を1行目に1個、2行目に2個、・・・、5行目に5個表示しなさい。ただし、以下のステートメントをそれぞれ1回だけ用いることとする。

- System.out.print("★");
- System.out.println();

**出力結果**

<img src="img/ex11.png" width="300">

<br><br>

## 演習12（ex12.java）
"★"を1行目に5個、2行目に4個、・・・、5行目に1個表示しなさい。ただし、以下のステートメントをそれぞれ1回だけ用いることとする。

- System.out.print("★");
- System.out.println();

**出力結果**

<img src="img/ex12.png" width="300">

<br><br>

## 演習13（ex13.java）
"★"を出力結果のような形に表示しなさい。ただし、以下のステートメントをそれぞれ1回だけ用いることとする。

- System.out.print("　");
- System.out.print("★");
- System.out.println();

**出力結果**

<img src="img/ex13.png" width="300">

<br><br>

## 演習14（ex14.java）
"★"を出力結果のような形に表示しなさい。ただし、以下のステートメントをそれぞれ1回だけ用いることとする。

- System.out.print("★");
- System.out.println();

**出力結果**

<img src="img/ex14.png" width="320">

<br><br>

## 演習15（ex15.java）
"★"を出力結果のような形に表示しなさい。ただし、以下のステートメントをそれぞれ1回だけ用いることとする。

- System.out.print("　");
- System.out.print("★");
- System.out.println();

**出力結果**

<img src="img/ex15.png" width="300">

<br><br>

## 演習16（ex16.java）
1行目に"1"を9個、2行目に"2"を8個、・・・9行目に"9"を1個を表示しなさい。

**出力結果**

```
111111111
22222222
3333333
444444
55555
6666
777
88
9
```

<br>

## 演習17（ex11.java）
演習11のex11.javaを修正する。printStar関数（引数あり／戻り値なし）を定義し、1行分の"★"を表示しなさい。5回のループの中でprintStar関数を呼び出す。

**出力結果**<br>※演習11と同様

<br>

## 演習18（ex18.java）
配列に格納されている数値を昇順（小さい値からだんだん大きい値になる順）に並べ替え、配列の中身を表示しなさい。並び替えは、隣り合う要素を最初から見ていき、大きさが逆であれば入れ替える、バブルソートとする。

```java
int[] scores = {65, 23, 47, 92, 53};
```

**出力結果**

```
23
47
53
65
92
```

<br><br><br>

<hr>

<a href="ans/ans.md">解答例</a>
