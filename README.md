# ECharts-Demo
## ECharts 埋坑之旅

### 1.双y轴对齐问题
默认情况下，echarts会根据数据进行自动渲染轴数据，合理安排大小。但是当双y轴情况下，各自轴线可能出现分割不均匀的情况。那在这时候可以通过自定义<b>min</b>、<b>max</b>、<b>interval</b>的值来进行固定设置。max设置为当前的最大值（或最大值向上的整数，规则自己定义）。

### 2.实现滑动效果
 dataZoom配置项用来设置滑动和放大缩小，type有两个值，'inside' 和 'slider'
 
### 3.移动端滑动效果
在项目中有一个类似keep的华东图标，单纯的通过echarts不能实现其功能所以通过给dom绑定touch事件来实现滑动的一系列操作，然后再重绘 echarts的canvas
