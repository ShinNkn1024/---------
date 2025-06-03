# ___まとめ___ 
## ___チートシート___



## 見出し
```
   # hello
　　　～
###### hello
```
# hello
## hello
### hello
#### hello
##### hello
###### hello


___
## 改行
```
いつも(半角スペース)(半角スペース)
ありがとう
```
いつも  
ありがとう


___
## 引用
```
> 引用
>> 多重引用
```
> 引用
>> 多重引用


___
## コード
```
```
↑これ  
`×3で囲む


___
## インラインコード
```
これは`ペン`です
```
これは`ペン`です


___
## 水平線
```
___
or
***
or
---

```
___
***
---


___
## リスト
### 箇条書き
```
-
or
+
or
*
を先頭に記述

- 箇条書き
+ 箇条書き
* 箇条書き
```
- 箇条書き
+ 箇条書き
* 箇条書き


___
## 番号
```
文字の前に1.を記述
自動的に番号がつく

1. 一番
1. 二番
1. 三番
```
1. 一番
1. 二番
1. 三番


___
# その他
## リンク

```
[表示文字](URL)の形でリンクに変換される

[Google](https://www.google.co.jp/)
[FlutterStudio](https://flutterstudio.app/)
```
[Google](https://www.google.co.jp/)  
[FlutterStudio](https://flutterstudio.app/)



# 強調
### 斜体
```
 *(文字)* 
or
 _(文字)_ 
```
私は *O型* です  
私は _さそり座_ です



### 太字
```
 **(文字)** 
or
  __ (文字)__ 
```
私は **2006年** 生まれです  
私は __10月24日__ 生まれです



## 斜体+太字
```
 ***(文字)*** 
or
 ___(文字)___ 
```
私は ***男*** です  
私は ___170cm___ です



## 打消し
```
 ~~(文字)~~ 
```
私は ~~こころ~~ です  
私は しん です



## Imamges 画像
```
リンク表記の先頭の!で画像と認識される


![](画像URL)


![ドラえもん](https://msp.c.yimg.jp/images/v2/FUTi93tXq405grZVGgDqG7eOnLcmQXcni-ZTPnGH_y_6GrPwwoWjC0YogA1I7BYWE9IpWzrU6AFrukm9ebEuGcw2C8bdV9mTV4av6tD69xPszzCbZENTza-YgU3U-_hFhWxamlc3fUVQpg9OVjrz7RQx0V7tfujTsouQqq-Jg-IaTtnWiVFvMmePQRje8cZjTILO2mYw-9qvIsm7OY9HKoD9PaMy_KcCzisAa2vjztNTEzTsFYIFzPEhgLSymVwMk5WJizU3IOS-_IDE5qTQG4Nk1FqJ9eE0Kz8G6BZUDmg=/doraemon.jpg)
```

![ドラえもん](https://msp.c.yimg.jp/images/v2/FUTi93tXq405grZVGgDqG7eOnLcmQXcni-ZTPnGH_y_6GrPwwoWjC0YogA1I7BYWE9IpWzrU6AFrukm9ebEuGcw2C8bdV9mTV4av6tD69xPszzCbZENTza-YgU3U-_hFhWxamlc3fUVQpg9OVjrz7RQx0V7tfujTsouQqq-Jg-IaTtnWiVFvMmePQRje8cZjTILO2mYw-9qvIsm7OY9HKoD9PaMy_KcCzisAa2vjztNTEzTsFYIFzPEhgLSymVwMk5WJizU3IOS-_IDE5qTQG4Nk1FqJ9eE0Kz8G6BZUDmg=/doraemon.jpg)



## Table表
```
-と|を使ってtableを作成する

| TH1 | TH2 |
----|----
| TD1 | TD3 |
| TD2 | TD4 |
```


| TH1 | TH2 |
----|----
| TD1 | TD3 |
| TD2 | TD4 |


```
| 左揃え | 中央揃え | 右揃え |
|:---|:---:|---:|
|1 |2 |3 |
|4 |5 |6 |
```


| 左揃え | 中央揃え | 右揃え |
|:---|:---:|---:|
|1 |2 |3 |
|4 |5 |6 |




___
# ___Flutter___ 
### リスト2-1
```
void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Flutter Demo',
      home: Text(
        'Hello, Flutter World!!',
        style: TextStyle(fontSize:32.0),
      ),
    );
  }
}
```



## main() 関数

* ```runApp(MyApp());```で```MyApp```ウィジェットをアプリをして起動


## MyApp クラス
* ```StatelessWidget``` を継承しており、状態をもたないウィジェット
* ```build()``` メソッドでUIを構築


## MaterialApp
* Flutterの基本的なアプリの土台となるウィジェット
* ```title``` プロパティでアプリのタイトルを設定


## home
* ```Text``` ウィジェットをホーム画面として設定
* フォントサイズを ```32.0``` に指定し、「Hello,FlutterWorld!!」と表示