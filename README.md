## 任务一知识清单
### 1.CSS3圆角
### 2.CSS3过渡
### 3.原生JS事件与DOM操作

## CSS3圆角
### border-radius  用于给边框添加圆角

![圆角原理](https://github.com/ciwei777/IFECSS301/blob/master/images/source1.png ''圆角的水平和垂直半径'')

#### 原理：
	想要真正玩转圆角，还是先要学习理解其原理
[border-radius原理解析](https://jingyan.baidu.com/article/1876c852549b2a890b1376bf.html)
[初步学习border-radius](https://www.cnblogs.com/s-b-b/p/5830119.html)
#### 语法：
 border-radius：[ <length> | <percentage> ]{1,4} [ / [ <length> | <percentage> ]{1,4} ]?
        <length>：用长度值设置对象的圆角半径长度。不允许负值
        <percentage>：用百分比设置对象的圆角半径长度。不允许负值
	示例：
	单个值 border-radius: 10px;  // 四个角的水平和垂直都是10px
	两个值 border-radius: 10px 20px; // 左上、右下的水平和垂直为10px，右上、左下的水平和垂直为20px
	三个值 border-radius: 10px 20px 30px; // 左上的水平垂直为10px，右上、左下的水平和垂直为20px，右下的水平和垂直为30px
	四个值 border-radius: 10px 20px 30px 40px; // 依次为左上、右上、右下、左下的水平和垂直
	'/'水平垂直分开写
								border-radius: 10px 20px 30px 40px / 40px 30px 20px 10px; // 以‘/’为分界，左侧为水平，右侧为垂直，顺序依次为左上、右上、右下、左下
	以上的border-radius其实为圆角的简写方式，完整写法是为四个角的八个方向分别设置值。
	例如： border-top-left:10px 20px; // 为左上角设置水平为10像素垂直为20像素的
	border-raidus值的单位也不限于px，还有em，%等
	
## CSS3过渡
### transtion 过渡效果
#### 语法：[transition基础语法](http://www.w3school.com.cn/cssref/pr_transition.asp)

transition: property duration timing-function delay;

transition 属性是一个简写属性，用于设置四个过渡属性：

transition-property 要过渡的属性 // 可以指定一个或多个属性
transition-duration 过渡时长 // 过渡动画总时长
transition-timing-function 速度函数 // linear ease ease-in ease-out ease-in-out cubic-bezier(n,n,n,n)
transition-delay 延迟时间 // 延迟多长时间开始

## 原生js事件以及Dom操作
获取DOM节点 
document.getElementById('xxx') // 通过id获取
document.getElementByClassName('xxx') // 通过类名获取 返回值是一个数组
document.getElementByTagName('xxx') // 通过标签名获取 返回值是一个数组
还有更多获取方式...
[获取DOM的八种方式](https://www.cnblogs.com/web-record/p/10131782.html)
[原生获取DOM的8中方式](https://www.cnblogs.com/web-record/p/10131782.html)

添加事件 
xxx.addEventListener('type', Fn)

以上是我完成此次任务所用到的全部知识点，只列出了一个大概，更多详细内容都可以百度。

​      
