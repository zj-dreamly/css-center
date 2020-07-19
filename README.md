### 水平居中布局

#### inline-block + text-align

- 浏览器兼容性好
- text-align属性具有继承性，导致子级元素的文本也是居中显示的

#### table + margin

- 只需要对子级元素进行设置就可以实现水平方向居中布局效果
- 如果子级元素脱离文档流，导致margin属性的值无效

#### absolute + transform

- 父级元素是否脱离文档流，不影响子级元素水平居中效果
- transform属性是CSS3中新增属性，浏览器支持情况不好

### 垂直居中布局

#### table-cell + vertical-align

- 浏览器兼容性好
- vertical-align属性具有继承性，导致父级元素的文本也是居中显示的

#### absolute + transform

- 父级元素是否脱离文档流，不影响子级元素水平居中效果
- transform属性是CSS3中新增属性，浏览器支持情况不好

### 居中布局

- table + margin实现水平方向居中，table-cell + vertical-align实现垂直方向居中
- absolute + transform实现水平方向和垂直方向居中

