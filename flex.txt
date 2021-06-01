flex(弹性盒,伸缩盒)
  --是css中的又一种布局手段，它主要用来代替浮动来完成页面的布局。
  --（float会使元素脱离文档流，导致父元素高度塌陷）
  --flex使元素具有弹性，让元素跟随父元素页面大小的改变而改变。
1.弹性容器
  --要使用弹性盒，必须先将元素设置为弹性容器
    通过 display 来设置弹性容器
      display:flex  块级
      display:inline-flex 行内
2.弹性元素
  --弹性容器的子元素是弹性元素。
  --一个元素可以同时是弹性容器和弹性元素。
flex-direction:容器中弹性元素的排列方式
默认值：row  水平排列
row-reverse 反向水平排列
column 纵向排列
column-reverse 反向纵向排列
主轴：弹性元素的排列方向为主轴。
侧轴：与主轴垂直的方向为侧轴。

弹性元素的属性：
	--flex-grow：指定弹性元素的伸展系数（可以单独给子元素设置）
	  默认值：0   当父元素有多余的空间时，子元素如何伸展。
	
	--flex-shrink：指定弹性元素的收缩系数（值越大，缩的越多）
	  默认值：1   当父元素..............,...........收缩。
	
	--flex-basis：元素在主轴上的基础长度
	  默认值：auto
	  如果主轴横向，则为元素的宽度；纵向，则高度。
	
	使用flex可以直接设置这三个值。

	--flex-wrap：是否换行
	  默认值：nowrap
	  wrap wrap-reverse
	
	--flex-flow：wrap和direction的简写属性

	--justify-content：如何分配主轴上的空白空间（主轴上的元素如何排列）
	  可选值：flex-start 元素沿主轴起边排列
	  	  flex-end   ..........终边....
		  center     居中排列
               ** space-around 空白分布到元素两侧   
		  space-evenly ..............单侧
	
	--align-items：元素在侧轴上如何对齐
	  ：stretch 默认值 将元素长度设置为相同的值（只是行与行之间的高度）
	  ：flex-start 元素不会拉伸，沿着侧轴起边对齐
	  ：flex-end   ......................终边....
	  : center     居中对齐
	  ：baseline   基线对齐

	--align-content：侧轴空白空间的分布（和justify-content可选值一样，只是方向不同，主轴侧轴）

	--align-self：用来覆盖当前弹性元素上的align-items

	--order：决定弹性元素的排列顺序
