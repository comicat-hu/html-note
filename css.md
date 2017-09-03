# **CSS**

(CSS 3)
[MDN CSS](https://developer.mozilla.org/zh-TW/docs/Web/CSS)

## **Index**

1. [CSS基本介紹](#css基本介紹)
2. [選擇器](#選擇器)

## CSS基本介紹

CSS(Cascading Style Sheets，層疊樣式表)，用來描述HTML、XML等文件外觀的樣式表，告訴瀏覽器文件中的元素該如何呈現出來。

* 籤入在HTML中時用\<style>標籤。

* 透過選擇器(selector)取得HTML element，並透過賦予屬性及值來改變樣式。(屬性: 屬性值;)

* 瀏覽器解析HTML成DOM(Document Object Model) Tree並同時解析CSS並套用到對應的元素上。

    ![CSS render](/img/rendering.png)

* 錯誤的語法或無效的設定會直接忽略

## 選擇器

* \* { } 選擇全部elements
* p { } 選擇全部p elements
* .classA { } 選擇全部有classA的elements
* #id-A { } 選擇id-A的element(id只能唯一，如果重複會發生不可預期的狀況)
* [attr] { } 選擇全部有attr屬性的elements
* [attr=val] { } 選擇全部有attr屬性並且值等於val的elements
* [attr~=val] { } 選擇全部有attr屬性並且值包含val的elements
* [attr|=val] { } 選擇全部有attr屬性並且值以val及val-開頭的elements
* [attr^=val] { } 選擇全部有attr屬性並且值以val開頭的elements
* [attr$=val] { } 選擇全部有attr屬性並且值以val結尾的elements
* [attr*=val] { } 選擇全部有attr屬性並且值包含val的elements
* [偽類Pseudo-class](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes) element:pseudo-class { } 用於選擇特定狀態下的elements
* [偽元素Pseudo-elements](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-elements) element::pseudo-element { } 用於選擇elements的特定部分  
    [pseudo element pseudo class difference](https://stringpiggy.hpd.io/pseudo-element-pseudo-class-difference/)
* A,B { } 選擇全部的A和B
* A B { } 選擇在A下層的所有B(後代)
* A > B { } 選擇在A子層的所有B(兒子)
* A + B { } 選擇全部A後面的那一個B(同層且相鄰)
* A ~ B { } 選擇全部A後面的的B(同層)
