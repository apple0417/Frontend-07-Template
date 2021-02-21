1.first-letter和first-line都作用于块级元；

2.first-letter:作用于第一行的首字符；

3.first-line：作用于第一行的所有字符；

 first-letter 可以设置 float 之类的，而 first-line 不行，是因为，首行字符数是不可控的，不同屏幕尺寸或者字体大小会影响首行渲染，比如在一段文字中使用first-letter，将首字母字体大小设置为行高的400%时