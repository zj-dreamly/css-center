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

### 两列布局

- 两列布局一般情况下是指定宽与自适应布局，两列中左列是确定的宽度，右列是自动填充满剩余所有空间的一种布局效果

#### 实现方式

- float + margin属性配合使用
- float + overflow属性配合使用
- display属性的table相关值使用

### 三列布局

- 三列布局一般情况下是指三列中的左边两列是确定的宽度，右边一列是自动填满剩余所有空间的一种布局效果

#### 实现方式

- float + margin属性配合使用
- float + overflow属性配合使用
- display属性的table相关值使用

### 圣杯布局

- 圣杯布局是来源于该布局效果类似圣杯而得名，简单来说，就是值三行三列布局

#### 核心

- 圣杯布局主要是实现中间主体部分中的左右定宽 + 中间自适应的布局效果

### 双飞翼布局

双飞翼布局最早是淘宝团队提出，是针对圣杯布局的优化解决方案，主要是优化了圣杯布局中开启定位的问题

### 等分布局

- 等分布局就是一行被分为若干列，每一列的宽度是相同值

#### 实现方式

- float
- display属性的值有关table实现等分布局效果

### 等高布局

- 一行被划分成若干列，每一列的高度都是相同的值

#### 实现方式

- display属性的值有关table实现等高布局效果
- padding + margin属性实现等高布局效果

### CSS3多列布局

#### column

- column-count：定义列的数量或者允许的最大列数
  - auto：默认值用于表示列的数量由其他CSS属性决定
  - number：必须是正整数，用于表示列的数量
- column-width：定义列的宽度或者列的最小宽度
  - auto：默认值用于表示列的宽度由其他CSS属性决定
  - number：必须是正整数，用于表示列的宽度

#### column-gap

column-gap属性用于设置列与列之间的间距，该属性需要为多列显示时的元素设置

- normal：用于表示使用浏览器的默认间距，默认为1em
- length：必须是正整数，用于定义列与列之间的间距

#### column-rule

column-rule用于列与列之间的边框，包括宽度，边框颜色以及样式

- column-rule-width：用于表示列与列之间的边框的宽度
- column-rule-color：用于表示列与列之间的边框颜色
- column-rule-style：用于表示列与列之间的边框样式