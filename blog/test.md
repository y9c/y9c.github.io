title: test
date: 2015-12-19 20:27:51
tags: [test, code]

---

# hehe

> hehe
这是一段引用
---- 阿尔伯特.爱因斯坦

#### 这是一条公式
$$ x^2 + y *100 $$

#### 牛逼的薛定谔方程
$\cos 2\theta = \cos^2 \theta - \sin^2 \theta =  2 \cos^2 \theta - 1$

{% gantt 测试甘特图 %}
    section section 1
    A task           :a1, 2014-01-01, 30d
    Another task     :after a1  , 20d
    section section 2
    Task in sec      :2014-01-12  , 12d
    anther task      : 24d
{% endgantt %}


```sequence
张三->李四: 嘿，小四儿, 写博客了没?
Note right of 李四: 李四愣了一下，说：
李四-->张三: 忙得吐血，哪有时间写。
```
```flow
st=>start: 开始
e=>end: 结束
op=>operation: 我的操作
cond=>condition: 确认？
st->op->cond
cond(yes)->e
cond(no)->op
```

