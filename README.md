# 浅谈Pandas样式
大家都知道 Excel 可以设定单元格格式，还支持单元格迷你图，其实 Pandas 也可以，本文参照 [Chris Moffitt](https://pbpython.com/author/chris-moffitt.html) 的 [Stylin’ with Pandas](https://pbpython.com/styling-pandas.html) 一文，为大家简单介绍一下 Pandas 如何实现 DataFrame 的样式设置，主要内容如下：

1. 设置 DataFrame 不同列的样式，如千分号、小数位数、货币符号、日期格式，百分比等；

2. 突出显示 DataFrame 中某一列里符合某些条件的数据，如，按不同颜色显示某列中的最大值与最小值；

3. 以不同渐变色展示每一行数据占总数据的比例大小，占比越大，颜色越深，占比越小，则颜色越浅；

4. 实现类似 Excel 迷你条形图的功能，根据数据大小，在单元格里显示迷你条形图；

5. 利用 Sparklines 支持库，配合 Pandas 绘制迷你走势图。需要先用 `pip install sparklines` 命令安装 Sparklines 支持库。
