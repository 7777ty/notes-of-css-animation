# CSS动画 

## 浏览器渲染原理

### 浏览器渲染过程
1. 根据HTML构建HTML树（DOM）
2. 根据CSS构建CSS树（CSSOM）
3. 将两棵树合并成一颗渲染树（render tree）
4. Layout布局（文档流、盒模型、计算大小和位置）
5. Paint绘制（把边框颜色、文字颜色、阴影等绘制出来）
6. Compose合成（根据层叠关系展示画面）
### 使用JS更新样式时的步骤
一共有三种更新方式：
1. JS/CSS>Style>Layout>Paint>Composite
2. JS/CSS>Style>Paint>Composite
3. JS/CSS>Composite

-----

## *[transform](https://developer.mozilla.org/zh-CN/docs/Web/CSS/transform)*

### 四个常用功能及其常用写法
* 位移 translate

```css
    translateX(<length-percentage>)
    translateY(<length-percentage>)
    translate(<length-percentage>,<length-percentage>)
    translateZ(<length-percentage>)
    translate3d(x,y,z)
```

tips: translate(-50%,-50%)可做绝对定位元素的居中。

* 缩放 scale

```css
scaleX(<number>)
scaleX(<number>)
scale(<number>,<number>)
```

tips:较少使用，因为会出现模糊。

* 旋转 rotate

```css
rotate([<angle>|<zero>])
rotateX([<angle>|<zero>])
rotateY([<angle>|<zero>])
rotateZ([<angle>|<zero>])

```
**[rotate3d](https://developer.mozilla.org/zh-CN/docs/Web/CSS/transform-function/rotate3d)** 较为复杂，请查看MDN文档。

* 倾斜 skew

```css
skewX([<angle>|<zero>])
skewY([<angle>|<zero>])
skew([<angle>|<zero>],[<angle>|<zero>])
```

-----------

## transition
**语法**
transition(过渡):属性名 时长 过渡方式 延迟
transition：left 200ms linear
具体可见：[transition MDN](https://developer.mozilla.org/zh-CN/docs/Web/CSS/transition)

---------

##animation
**语法**
animation:时长|过渡方式|延迟|次数|方向|填充模式|是否暂停|动画名；

具体可见：[animation MDN](https://developer.mozilla.org/zh-CN/docs/Web/CSS/animation)# notes-of-css-animation
