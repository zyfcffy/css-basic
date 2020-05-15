## 需求说明

### 完成下列选择题

1.在下列选择器中，哪一个代表 section class 里面的所有 title class?

<input type="radio" name="Q1" value="A"> <lable>.section .title {}</lable> 
 <br>
<input type="radio" name="Q1" value="B"> <lable>.section.title {}</lable>  
<br>
<input type="radio" name="Q1" value="C"> <lable>.section, .title {}</lable>  
<br>
<input type="radio" name="Q1" value="D"> <lable>.section > .title {}</lable>  
<br>
<br>

2.在下列选择器中，哪一个代表 section class 内部紧邻的 title class?

<input type="radio" name="Q2" value="A"> <lable>.section .title {}</lable> 
 <br>
<input type="radio" name="Q2" value="B"> <lable>.section.title {}</lable>  
<br>
<input type="radio" name="Q2" value="C"> <lable>.section, .title {}</lable>  
<br>
<input type="radio" name="Q2" value="D"> <lable>.section > .title {}</lable>  
<br>
<br>


3.在下列选择器中，哪一个代表同一个元素同时拥有 section 和 title 两个class?

<input type="radio" name="Q3" value="A"> <lable>.section .title {}</lable> 
 <br>
<input type="radio" name="Q3" value="B"> <lable>.section.title {}</lable>  
<br>
<input type="radio" name="Q3" value="C"> <lable>.section, .title {}</lable>  
<br>
<input type="radio" name="Q3" value="D"> <lable>.section > .title {}</lable>  
<br>
<br>


4.在下列选择器中，哪一个代表 section 和 title 两个class 设置相同样式?

<input type="radio" name="Q4" value="A"> <lable>.section .title {}</lable> 
 <br>
<input type="radio" name="Q4" value="B"> <lable>.section.title {}</lable>  
<br>
<input type="radio" name="Q4" value="C"> <lable>.section, .title {}</lable>  
<br>
<input type="radio" name="Q4" value="D"> <lable>.section > .title {}</lable>  
<br>
<br>


5.在下列CSS选择器中，优先级从高到低是：
```
<div class="section">
    <h1 id="title" class="title">title</div>
</div>

A)  .section .title { color:red; }
B)  #title { color:green; }
C)  .title { color:yellow !important; }
D)  .section > h1 { color:blue; }
```
<input type="radio" name="Q5" value="A"> <lable> B > C > D > A </lable> 
 <br>
<input type="radio" name="Q5" value="B"> <lable> C > B > A > D </lable>  
<br>
<input type="radio" name="Q5" value="C"> <lable> D > B > A > C</lable>  
<br>
<input type="radio" name="Q5" value="D"> <lable> 以上都不对 </lable>  
<br>
<br>
<br>
  
  
## 本练习知识点

- CSS can change the look of HTML elements. In order to do this, CSS must select HTML elements, then apply styles to them.
- CSS can select HTML elements by tag, class, or ID.
- Multiple CSS classes can be applied to one HTML element.
- Classes can be reusable, while IDs can only be used once.
- IDs are more specific than classes, and classes are more specific than tags. That means IDs will override any styles from a class, and classes will override any styles from a tag selector.
- Multiple selectors can be chained together to select an element. This raises the specificity, but can be necessary.
- Nested elements can be selected by separating selectors with a space.
- The `!important` flag will override any style, however it should almost never be used, as it is extremely difficult to override.
- Multiple unrelated selectors can receive the same styles by separating the selector names with commas.

