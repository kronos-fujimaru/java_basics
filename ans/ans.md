# Java入門 演習問題（解答例）

## 演習1（ex01.java）

```java
class ex01 {
    public static void main(String[] args) {
        int a = 10;
        int b = 20;

        int c = a;
        a = b;
        b = c;

        System.out.println("変数a = " + a);
        System.out.println("変数b = " + b);
    }
}
```

<br>

## 演習2（ex02.java）

```java
class ex02 {
    public static void main(String[] args) {
        int score = 80;
        System.out.println("点数：" + score + "点");

        if (score >= 80) {
            System.out.println("優良");
        } else if (score >= 50) {
            System.out.println("良");
        } else if (score >= 30) {
            System.out.println("可");
        } else {
            System.out.println("不可");
        }
    }
}
```

<br>

## 演習3（ex03.java）

```java
class ex03 {
    public static void main(String[] args) {
        int num = 231;

        if (num % 3 == 0) {
            System.out.println("3の倍数");
        }
        if (num % 5 == 0) {
            System.out.println("5の倍数");
        }
        if (num % 7 == 0) {
            System.out.println("7の倍数");
        }
        if (num % 11 == 0) {
            System.out.println("11の倍数");
        }
    }
}
```

<br>

## 演習4（ex04.java）

```java
class ex04 {
    public static void main(String[] args) {
        int age = 25;
        int license = 1;

        if (age < 20 || license == 1) {
            System.out.println("1200円");
        } else if (age >= 65) {
            System.out.println("1500円");
        } else {
            System.out.println("1800円");
        }
    }
}
```

<br>

## 演習5（ex05.java）

```java
class ex05 {
    public static void main(String[] args) {
        int sum = 0;
        for (int i = 1; i <= 100; i++) {
            sum += i;
            System.out.println(sum);
        }
    }
}
```

<br>

## 演習6（ex06.java）

```java
class ex06 {
    public static void main(String[] args) {
        int sum = 0;
        for (int i = 1; i <= 100; i++) {
            if (i % 2 == 0) {
                sum += i;
            }
        }
        System.out.println("合計：" + sum);
    }
}
```

<br>

## 演習7（ex07.java）

```java
class ex07 {
    public static void main(String[] args) {
        int[] scores = {80, 72, 64, 81, 90, 56, 79, 92, 43, 78};
        int max = scores[0];

        for (int i = 1; i < scores.length; i++) {
            if (max < scores[i]) {
                max = scores[i];
            }
        }
        System.out.println("最大：" + max);
    }
}
```

<br>

## 演習8（ex08.java）

```java
class ex08 {
    public static void main(String[] args) {
        int[] values = {50, 23, -64, 38, -10, 13, 41, -35, -5, 26};
        int sum = 0;

        for (int value : values) {
            if (value < 0) {
                value = value * -1;
            }
            sum += value;
        }
        System.out.println("合計：" + sum);
    }
}
```

<br>

## 演習9（ex09.java）

```java
class ex09 {
    public static void main(String[] args) {
        int sum = 0;
        for (String value : args) {
            sum += Integer.parseInt(value);
        }
        System.out.println("合計：" + sum);
    }
}
```

<br>

## 演習10（ex10.java）

```java
class ex10 {
    public static void main(String[] args) {
        for (int i = 0; i < 3; i++) {
            for (int j = 0; j < 5; j++) {
                System.out.print("★");
            }
            System.out.println();
        }
    }
}
```

<br>

## 演習11（ex11.java）

```java
class ex11 {
    public static void main(String[] args) {
        for (int i = 1; i <= 5; i++) {
            for (int j = 0; j < i; j++) {
                System.out.print("★");
            }
            System.out.println();
        }
    }
}
```

<br>

## 演習12（ex12.java）

```java
class ex12 {
    public static void main(String[] args) {
        for (int i = 0; i < 5; i++) {
            for (int j = 0; j < 5 - i; j++) {
                System.out.print("★");
            }
            System.out.println();
        }
    }
}
```

<br>

## 演習13（ex13.java）

```java
class ex13 {
    public static void main(String[] args) {
        for (int i = 1; i <= 5; i++) {
            for (int j = 0; j < 5 - i; j++) {
                System.out.print("　");
            }
            for (int j = 0; j < i; j++) {
                System.out.print("★");
            }
            System.out.println();
        }
    }
}
```

<br>

## 演習14（ex14.java）

```java
class ex14 {
    public static void main(String[] args) {
        int[] numStars = {8, 4, 10, 6};
        for (int i = 0; i < args.length; i++) {
            for (int j = 0; j < numStars[i]; j++) {
                System.out.print("★");
            }
            System.out.println();
        }
    }
}
```

<br>

## 演習15（ex15.java）

```java
class ex15 {
    public static void main(String[] args) {
        int star = 1;
        for (int i = 1; i <= 5; i++) {
            for (int j = 0; j < 5 - i; j++) {
                System.out.print("　");
            }
            for (int j = 0; j < star; j++) {
                System.out.print("★");
            }
            star += 2;
            System.out.println();
        }
    }
}
```

<br>

## 演習16（ex16.java）

```java
class ex16 {
    public static void main(String[] args) {
        for (int i = 1; i <= 9; i++) {
            for (int j = 0; j < 10 - i; j++) {
                System.out.print(i);
            }
            System.out.println();
        }
    }
}
```

<br>

## 演習17（ex11.java）

```java
class ex11 {
    static void printStar(int count) {
        for (int i = 0; i < count; i++) {
            System.out.print("★");
        }
        System.out.println();
    }

    public static void main(String[] args) {
        for (int i = 1; i <= 5; i++) {
            printStar(i);
        }
    }
}
```

<br>

## 演習18（ex18.java）

```java
class ex18 {
    public static void main(String[] args) {
        int[] scores = {65, 23, 47, 92, 53};

        for (int i = 1; i <= scores.length; i++) {
            for (int j = 0; j < scores.length - i; j++) {
                if (scores[j] > scores[j + 1]) {
                    int temp = scores[j + 1];
                    scores[j + 1] = scores[j];
                    scores[j] = temp;
                }
            }
        }

        for (int score : scores) {
            System.out.println(score);
        }
    }
}
```
