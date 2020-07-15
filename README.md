## 関数を作る  



### ①仕様を考える　（今回の例題:苗字と名前の文字列を２つ取って、間にスペースを入れ、くっつけて返す。）
・どのような処理をさせたいか



### ②関数名を考える
・関数作成時には、関数名の前に"let"が必要なため、その後ろへ関数名を入れる。  
　(今回は"getName"を関数名とする。)

```
let getName

```



### ③パラメーターの数を考える
・処理に必要なパラメーターの数を考え、関数名とイコールで繋がる（　）を作る。（　）の中にはパラメーターの数に合わせて区切りのコンマ( , )が必要となる。

```
let getName =　( , ) => {

}
```



### ④パラメーターにわかりやすく、関連があるような名前を作る
(今回は"lastname"と"firstname"をパラメーターとする。※わかりやすくするために、名前の前にp_とつけておく。)  
(パラメーターはその関数内部でしか使用できない変数であり、ローカル変数という。）

```
let getName =　(p_lastname,p_firstname) => {

}
```



### ⑤戻り値の変数を作る
・戻り値と同じ型で、初期値にする  
(オブジェクトの場合は「null」,数字の場合は「0」,文字の場合は空文字「""」にしておく)  
(今回は文字列のため空文字「""」とする。 ※戻り値だとわかりやすくするため、変数名の前にr＿とつけておく)

```
let getName = (p_lastname,p_firstname) => {
    let r_name = "";
 }
```

### ⑥数行改行
・戻り値の変数に結果を入れる為のコードを書くスペースを空けておく

```
let getName = (p_lastname,p_firstname) => {
    let r_name = "";
   
   
 }
```



### ⑦戻り値の変数をリターンする

```
let getName = (p_lastname,p_firstname) => {
    let r_name = "";
   
   
    return r_name;
 }
```



### ⑧仕様を満たすように処理を作る
・⑥で改行したスペースに、戻り値の変数に結果を入れる為のコードを書く  
(今回は　name = p_lastname + " " + p_firstname;　とする)

```
let getName = (p_lastname,p_firstname) => {
    let r_name = "";
    name = p_lastname + " " + p_firstname;
    return r_name;
 }
```




## 関数を使う



### ①関数名を書く
・使いたい関数の関数名を書く

```
getName
```



### ②関数名の後ろに( )を作る
```
getName();
```



### ③( )の中に変数もしくは値を入れる
・値を入れる場合
```
getName("ikeda","karen");
```

・変数を入れる場合  
（新たに変数を作成する）
```
let lastname = "ikeda";
let firstname = "karen";
getName(lastname , firstname);
```
