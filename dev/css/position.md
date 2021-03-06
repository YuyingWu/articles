# position

`static`是`position`属性的默认值，表示元素在文档布局里面的正常位置。静态元素不能指定`top`、`left`等表示位置的属性。

`absolute`表示当前元素相对于它的容器元素的绝对位置。它独立于其他元素，不再是正常内容布局的一部分。绝对定位元素的容器元素，是它最近一层不是`static`布局的元素，如果没有的话，就是相对于`document`元素的布局。

`fixed`表示元素位置相对于浏览器窗口是固定的。这个元素总是可见，而且不会随着页面滚动而滚动。固定定位的元素，独立于其他元素，不是正常内容布局的一部分。

`relative`表示元素的位置是相对于它的正常位置。它依然属于内容布局的一部分，周边元素不受它的位置改变的影响。

## z-index

`z-index`表示元素重叠时的层次关系，默认时是0。

由于静态布局的元素不会产生重叠，所以该属性对静态元素无效，但是可以通过调整重叠元素的`z-index`属性（正值表示在上方，负值表示在下方），达到想要的效果。
