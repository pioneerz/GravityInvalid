# GravityInvalid

## 这是个demo

![演示图](https://github.com/pioneerz/layer_list/blob/master/layer_list.png)

从这张图可以看出 当linearlayout的orientation=“vertical”时在Textview里面设置layout_gravity=“bottom” 没有生效
其实如果我们再多测试测试的话，我们会发现：
  1.当orientation = “vertical”时 
        layout_gravity=“top”或者“bottom” 都是无效的。
  2.当orientation = “horizontal”时
        layout_gravity="left"或者"right" 都是无效的

这是为什么？
  因为linearlayout是线性布局，按照从上到下或者从左到右布局子view，如果对应layout_gravity生效的话，会造成布局混乱。
