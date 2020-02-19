# CSS Summary

CSS is invented by Hakon Wium Lie, who’s a colleague of Duke Lee. 
why is css so powerful? because it’s a cascading style sheet, cascading. You can select the same element with different selectors 
the most prevalent, widely used css version is css 2.1, which is released between 2004-2011, 7 years under constant development. 

to see if you can use a certain css feature or command on a web browser, that is, if the browser is compatible, go to caniuse.com to check 

to learn css completely is virtually impossible

basic syntax:
select {
    attribute: value; 
    /*comments*/
}

@charset “UTF-8”;
@import url();
@media 

charset must be on the first line. 
border testing, putting border in the selector at different places to see which line is not run correctly 

there are no high-level errors in css, just dumb stupid errors. 
so, check yo self.

freepik, free PSD web
dribble.com 
best way to practice css and html is to use actual websites. 
start with mobile, because mobile is smaller and easier to actualize. 

normal flow, the flow of elements in the document, from left right, from top to bottom. 
inline elements goes from left from right. when a span element reaches the right border, it will continue on the next line instead of moving its entirety to the second line. 
block elements go from top to bottom
inline block displays every element in its entirety, if the width of the current line is not enough, it goes to the next line.

the latest version of html 5, there’s no two-way categorization of inline and block elements. 
all the elements can be block or inlilne

just don’t embed block elements in inline element tags
the default width of block element is auto, meaning that, taking as much space as possible
don’t use width = 100%, unless it’s absolutely necessary. 

the height of inline elements is determined by the line-height. Padding might increase the size of the border, but it does not change the actual line-height. It has nothing to do with height. 

div wraps all the element inside the div tag that’s within the normal flow

to jump out of normal flow:
position: absolute 
float: left or right

盒模型
css的一个概念
content box 内容盒模型
border box 边框盒模型
用box-sizing来选择这两种模型
border box中width是指的边框之间的距离，边框的最左边到最右边
content box中的width指的是内容的宽度，就是content的宽度

css盒模型标准回答
css盒模型分两种，一种是content box，另一种是border box。区别在于
content box的width只是包涵content
border box的width包含到border，分别是border，padding，和content
border box更好用一点，因为比较好计算距离

margin 合并
重复的margin会合并，别问为什么
如果想不合并margin，将display换成inline block
合并的时候只有上下重叠，但是左右没有重叠
想要child和parent上下的margin不重叠，三种方式：
加个padding
加个border
加个overflow：hidden

css layout 
left, mid, right, or top, mid bottom 
two kinds of layouts: 
fixed-width layout and responsive layout

pages are responsive when you made it.
so when people say, oh i need to make my page responsive, it’s just bull

or you can make two kinds of layout. Fixed-width on computers, and responsive on mobile device. 

reset format code:
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

text-align: center not only allows the text inside a div to align center, but also other elements as well. 

嵌套关系的margin
如果son的margin设置顶部，那么father也会受到影响
解决方案：
1. father border-top： transparent
2. father padding-top: 1px
3. father overflow: hidden 

css position
in a div, background is at the bottom, then border, then the text content. 
background, border, 块级子元素，浮动元素，内联子元素

positions: 
static (default), relative, absolute, fixed, sticky

relative: the space that the element is taking does not change, but where the element  appears changes. 
relative is relative to your original position, while absolute is absolute to the parent element 
white-space: 文字内容是否换行，nowrap就是不准换行

try not to use position fixed on mobile pages.

four important scenarios that creates a new z-index: z-index = 0; flex, opacity, and transform.
csstriggers.com it’s a website that tells you which part has been triggered during rendering. 
