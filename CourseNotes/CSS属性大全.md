
@[TOC](目录)

# 文本属性

1 字体样式 {font:font-style font-variant font-weight font-size font-family}
2 字体类型 {font-family:”字体1″,”字体2″,”字体3″,…} 常用字体：“Courier New”, Courier, monospace, “Times New Roman”, Times, serif, Arial, Helvetica, sans-serif, Verdana
3 字体大小 {font-size:数值|inherit| medium| large| larger| x-large| xx-large| small| smaller| x-small| xx-small}
4 字体风格 {font-style:inherit|italic|normal|oblique(偏斜体)}
5 字体粗细  {font-weight:100-900|bold|bolder|lighter|normal;}
6 字体颜色  {color:数值;}
7 阴影颜色 {text-shadow:16位色值}
8 字体行高  {line-height:数值|inherit|normal;}
9 字 间 距  {letter-spacing:数值|inherit|normal}
10 单词间距 {word-spacing:数值|inherit|normal}
11 字体变形 {font-variant:inherit|normal|small-cps(小型大写字母) }
12 英文大小写转换 {text-transform:inherit|none|capitalize(首字母大写) |uppercase(大写) |lowercase}
13 字体变形 {font-size-adjust:inherit|none}
14 字体 {font-stretch:condensed|expanded|extra-condensed|extra-expanded|inherit|narrower|normal| semi-condensed|semi-expanded|ultra-condensed|ultra-expanded|wider}
15 修饰{text-decoration: underline(下划线)| overline(上划线)| line-through(删除线)| blink(闪烁)}
16 段首空格  {text-indent:数值|inherit}
17 水平对齐 {text-align:left|right|center|justify}
18 垂直对齐 {vertical-align:inherit|top|bottom|text-top|text-bottom|baseline|middle|sub|super}
19 书写方式 {writing-mode:lr-tb|tb-rl}



# 背景属性
简写方法 background:#000 url(..) repeat fixed left top;
1 背景颜色 {background-color:数值}
2 背景图片 {background-image: url(URL)|none}
3 背景重复 {background-repeat:inherit|no-repeat|repeat|repeat-x|repeat-y}
4 背景固定 {background-attachment:fixed|scroll}
5 背景定位 {background-position:数值|top|bottom|left|right|center}
6 背影样式 {background:背景颜色|背景图象|背景重复|背景附件|背景位置}
7 背景透明 {background:transparent; /*透视背景*/}

# 区块属性
字间距letter-spacing: normal; 数值
对齐text-align: justify;(两端对齐) left;(左对齐) right;(右对齐) center;(居中)
缩进text-indent: 数值px;
垂直对齐vertical-align: baseline;(基线) sub;(下标) super;(下标) top; text-top; middle; bottom; text-bottom;
词间距word-spacing: normal; 数值
空格white-space: pre;(保留) nowrap;(不换行)
显示display:block;(块) inline;(内嵌) list-item;(列表项) run-in;(追加部分) compact;(紧凑) marker;(标记) table; inline-table; table-raw-group; table-header-group; table-footer-group; table-raw; table-column-group; table-column; table-cell; table-caption;(表格标题)

# 方框属性
width:; height:; float:; clear:both; margin:; padding:;     顺序：上右下左

1 边界留白 {margin:margin-top margin-right margin-bottom margin-left}
2 补白 {padding:padding-top padding-right padding-bottom padding-left}
3 边框宽度 {border-width:border-top-width border-right-width border-bottom-width border-left-width}
宽度值： thin|medium|thick|数值
4 边框颜色 {border-color:数值 数值 数值 数值}数值：分别代表top、right、bottom、left颜色值
5 边框风格 {border-style:none|hidden|inherit|dashed|solid|double|inset|outset|ridge|groove}
6 边框 {border:border-width border-style color}
上 边 框 {border-top:border-top-width border-style color}
右 边 框 {border-right:border-right-width border-style color}
下 边 框 {border-bottom:border-bottom-width border-style color}
左 边 框 {border-left:border-left-width border-style color}
7 宽度 {width:长度|百分比| auto}
8 高度 {height:数值|auto}
9 漂浮 {float:left|right|none}
10 清除 {clear:none|left|right|both}



# 列表属性
## list-style

类型 list-style-type:none;/*不编号*/ decimal; /*阿拉伯数字*/ lower-roman; /*小写罗马数字*/ upper-roman; /*大写罗马数字*/ lower-alpha; /*小写英文字母*/ upper-alpha; /*大写英文字母*/ disc; /*实心圆形符号*/ circle; /*空心圆形符号*/ square; /*实心方形符号*/
位置 list-style-position: outside;/*凸排)*/ /*inside(缩进)*/;
图像 list-style-image: url(..)/*图片式符号*/;



# 定位属性
## position

Position: absolute; relative; static; fixed

## visibility

visibility: inherit; visible; hidden;

## overflow

overflow: visible; hidden; scroll; auto;

## clip

clip: rect(12px,auto,12px,auto) (裁切)







# 链接与鼠标属性
## **a**

a /*所有超链接*/
a:link /*超链接文字格式*/
a:visited /*浏览过的链接文字格式*/
a:active /*按下链接的格式*/
a:hover /*鼠标转到链接*/

## **cursor**

链接手指 CURSOR: hand
十字体 cursor:crosshair
箭头朝下 cursor:s-resize
十字箭头 cursor:move
箭头朝右 cursor:move
加一问号 cursor:help
箭头朝左 cursor:w-resize
箭头朝上 cursor:n-resize
箭头朝右上 cursor:ne-resize
箭头朝左上 cursor:nw-resize
文字I型 cursor:text
箭头斜右下 cursor:se-resize
箭头斜左下 cursor:sw-resize
漏斗 cursor:wait
光标图案(IE6)  p {cursor:url(“光标文件名.cur”),text;}



# 分类列表
序号 中文说明 标记语法
1 控制显示 {display:none|block|inline|list-item}
2 控制空白 {white-space:normal|pre|nowarp}
3 符号列表 {list-style-type:disc|circle|square|decimal|lower-roman|upper-roman|lower-alpha|upper-alpha|none}
4 图形列表 {list-style-image:URL}
5 位置列表 {list-style-position:inside|outside}
6 目录列表 {list-style:目录样式类型|目录样式位置|url}
7 鼠标形状 {cursor:hand|crosshair|text|wait|move|help|e-resize|nw-resize|w-resize|s-resize|se-resize|sw-resize}


