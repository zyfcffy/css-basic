## CSS 学习参考

### What is CSS?

CSS, or Cascading Style Sheets,  is a language that web developers use to *style* the HTML content on a web page. CSS can define styles and change the layout and design of a sheet. (colors, font types, font sizes, shadows, images, element positioning, and more)



### Add CSS Stylesheet to HTML Page

**1. Use `<link>` Element** (recommended)

CSS code can be written in its own files to keep it separate from the HTML code. The extension for CSS files is **.css**. These can be linked to an HTML file using a `<link>` tag in the `<head>` section.

The `<link>` element is used to link HTML documents to external resources like CSS files. It commonly uses:

- `href` attribute to specify the URL to the external resource
- `rel` attribute to specify the relationship of the linked document to the current document
- `type` attribute to define the type of content being linked

```html
<head>
  <link href="style.css" type="text/css" rel="stylesheet">
</head>
```



**2. Write CSS in HTML File**

CSS code can be written in an HTML file by enclosing the code in `<style>` tags. Code surrounded by `<style>` tags will be interpreted as CSS syntax.

```css
head>
  <style>
    h1 {
      color: blue;
    }
  </style>
</head>
```



**3. Inline Style**

CSS styles can be directly added to HTML elements by using the `style` attribute in the element’s opening tag. Each style declaration is ended with a semicolon. Styles added in this manner are known as *inline styles*.

```html
<h2 style="text-align: center;">Centered text</h2>
<p style="color: blue; font-size: 18px;">Blue, 18-point text</p>
```



### CSS Expression

```css
selector {
  property : value
}
```



### CSS Selectors

- **标签选择器 **（h1, p, div ...）

  ```css
  /* Selects all p elements */
  p {
  }
  ```

- **类选择器** （can be **reusable** and applied to many elements）

  ```css
  /* Selects all elements with class="column" */
  .column {
  }
  ```

- **ID选择器** （should be **unique** and used to style only a single element）

  ```css
  /* Selects element with id="first-item" */
  #first-item {
  } 
  ```

- 伪类选择器 （a:hover ...）

  ```css
  a:hover {
  }
  ```

- 伪元素选择器  

  ```css
  /* selects the first line of P element */
  p::first-line {
  }
  ```

- 分组选择器 

  ```css
  /* the text for both `h1` and `h2` is set to red. */
  h1, h2 {
    color: red;
  }
  ```

- 子选择器 （ .header > h1 ）

- 包含（后代）选择器 （ .header  h1 ）

- 属性选择器 （ input[disable] ）

- 通配选择器 （ * ）



### CSS 属性书写顺序 （参考）

1. 位置属性 （position, top, right, z-index, display ...）
2. 大小 (width, height, padding, margin)
3. 文字系列 (font, color, text-align, line-height, letter-spacing ...)
4. 背景 (background, border ...)
5. 其他 (animation, transition ...)



### CSS Cascade Order (层叠顺序)

详细介绍：http://w3help.org/zh-cn/kb/005/#header_3



### CSS Selector's Specificity （选择器的权重计算）

The most specific selector type is the **ID selector**, followed by **class selectors**, followed by **tag selectors**.

The CSS `!important` rule is used on declarations to override any other declarations for a property and ignore selector specificity. However, generally it is good to avoid using `!important` as bad practice.

选择器特殊性的计算规则: http://w3help.org/zh-cn/kb/005/#header_4



### CSS inheritance  (继承)

部分属性可以被子元素继承



### CSS 盒模型 （box model）

http://w3help.org/zh-cn/kb/006/

https://developer.mozilla.org/zh-CN/docs/Web/CSS/CSS_Box_Model/Introduction_to_the_CSS_box_model



## 调试 CSS 

https://developer.mozilla.org/zh-CN/docs/Learn/CSS/Building_blocks/Debugging_CSS
