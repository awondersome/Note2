# Note2
整理后的笔记


### http封装

业务ts应该订阅一个observable，可以独立处理成功和错误回调

``http.post(url, data).subscribe``
``api.post(data).subscribe()``

api服务ts应该接收一个observable并返回一个observable，统一封装api的url

``return this.http.post(url, data)``

http服务ts返回一个observable


angular ng-zorro ng-alain ionic


## :（first | last)-child

*p:first-child 选择p的同级元素的(第一个 | 最后一个)，且这个元素必须是同类型*
*.class:first-child 选择.class所在元素的同级元素的(第一个 | 最后一个)，且这个元素必须是同类型，且这个元素必须得有.class*

```
p:first-child{
  color: red
}

<span>span1</span>
<p>
  p1
  <p>p2</p>
  <p>p3</p>
</p>
<p>p4</p>

// p2为red，p1不为red // p测试有个bug，p不能包含块级元素
```

```
.red:first-child{
  color: red
}

<p>p1</p>
<p class="red">
  p2
  <p class="red">p3</p>
  <span class="red">span1</span>
</p>
<p class="red">p4</p>

// p3为red，p1和span1都不为red // p测试有个bug，p不能包含块级元素
```


## :（first | last | nth)-of-type

*p:first-of-type 选择p的同级同类型元素的(第一个 | 最后一个 | 第n个)*
*.class:first-of-type 选择.class所在元素的同级同类型元素的(第一个 | 最后一个 | 第n个)，且这个元素必须得有.class*
*总结：.class:first-of-type 可以替代child，加类名可以防止影响下级同类型元素*

```
p:first-of-type{
  color: red
}

<span>span1</span>
<p>
  p1
  <p>p2</p>
  <p>p3</p>
</p>
<p>p4</p>

// p1和p2为red // p测试有个bug，p不能包含块级元素
```

```
.red:first-of-type{
  color: red
}

<span>span1</span>
<p>p1</p>
<p class="red">
  p2
  <p class="red">p3</p>
  <span class="red">span2</span>
</p>
<p class="red">p4</p>

// p3和span2为red，p2都不为red // p测试有个bug，p不能包含块级元素
```


