# **HTML**

(HTML 5)

[MDN HTML](https://developer.mozilla.org/zh-TW/docs/Web/HTML)  
[W3SCHOOLS HTML](https://www.w3schools.com/html/)  
[DevDocs HTML](http://devdocs.io/html/)  
[HTML Style](https://www.w3schools.com/html/html5_syntax.asp)  
[HTML validator](https://validator.w3.org/)  

## **Index**

1. [HTML基本介紹](#HTML基本介紹)
2. [Metadata in HTML head](#Metadata&nbsp;in&nbsp;HTML&nbsp;head)

## HTML基本介紹

HTML(HyperText Markup Language，超文字標記語言)

* 用來定義網頁的內容，但不定義網頁的功能。

* 由許多元素(element)組成，元素間可以巢狀嵌入。

    一個元素基本包含:
    ![HTML element](https://mdn.mozillademos.org/files/9347/grumpy-cat-small.png)

* tag基本上不分大小寫

* block element & inline element:

    + block element會在頁面上形成新的可視區域，ex. \<h1>, \<p>...等。
    + inline element通常會包含在block element內，不會造成新段落出現，ex. \<a>, \<em>, \<strong>...等。

* 有些元素只有一個tag(只有opening tag)，像是\<img>...等。

* 元素可以添加屬性(attribute)，屬性與元素或屬性間需空一格

    + 屬性名稱="屬性值"
    + 一些boolean的屬性可以簡寫，ex. disabled="disabled"可以直接寫成disabled

* 通常完整的HTML結構會包括:

        <!DOCTYPE html>
        <html>
        <head>
            <meta charset="utf-8">
            <title>My Web</title>
        </head>
        <body>
            <p>Hello World!</p>
        </body>
        </html>

    + doctype: 定義文件格式，大小寫無異
    + html: root element，整個頁面的最外層
    + head: 這裡放不直接顯示在頁面的資料及設定
    + meta charset: 定義使用的文字集
    + title: 定義頁面的標題(顯示在頁籤)
    + body: 頁面的可視區域

* 瀏覽器解析HTML時會將連續的空白省略至一個，省略所有換行，還有一些特定的字元，所以必須使用特殊的編碼來達成。[html 特殊字元編碼對照表](http://wywu.pixnet.net/blog/post/26889798-%5B%E9%9B%BB%E8%85%A6%5D-%E7%89%B9%E6%AE%8A%E5%AD%97%E5%85%83-html-%E7%B7%A8%E7%A2%BC%E5%B0%8D%E7%85%A7%E8%A1%A8)

* [應避免過時的語法](https://developer.mozilla.org/zh-TW/docs/Web_%E9%96%8B%E7%99%BC/Historical_artifacts_to_avoid)

## Metadata&nbsp;in&nbsp;HTML&nbsp;head

* 指定文字編碼

        <meta charset="utf-8">

* 設定author和description

    設定description有助於SEO，而且這段字會被用在搜尋結果

        <meta name="author" content="Comi">
        <meta name="description" content="this is a test web">

* 可以設定網站縮圖，ex. Facebook制訂的協議[Open Graph protocol](http://ogp.me/)

* 設定icon

        <link rel="shortcut icon" href="favicon.ico" type="image/x-icon">

* 設定語言

        <html lang="zh-TW">

* link css file和載入javascript

* 加入viewport(RWD的基本要素)

        <meta name="viewport" content="width=device-width, initial-scale=1.0">