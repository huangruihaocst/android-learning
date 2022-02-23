# Notes
- Android Studio中修改Layout的地方的Design界面，在GUI里修改一些属性值有时候会不work，这不一定是修改得不对，有可能是bug，在Code的tab修改就work了。
- Image, `Drawable`, `ImageView`不一定有相同大小。在`ImageView`里设置`layout_width`或者`layout_height`为`WRAP_CONTENT`实际是设置wrap了`Drawable`，而`Drawable`可能会比图片本身多个白边（上下或者左右），从而导致`ImageView`看起来比图片本身多个白边。如果要`ImageView`和图片本身比例完全相同，可以设置`adjustViewBounds`为`true`。细节可以看[这篇文章](https://www.jianshu.com/p/ad8d3987d560)。
