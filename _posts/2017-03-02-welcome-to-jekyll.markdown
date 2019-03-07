---
layout: post
title: 1、es6
date: '2017-03-02 17:05:13 +0000'
categories: jekyll update
published: true
---
一、var的问题
  a、没有块级作用域
  b、不能重复命名变量
  c、不能命名常量
  d、var在for循环中标记变量共享，一般会在循环中使用的i会被共享，其实质上也是由于没有块级作用域造成的。
二、常量 const
  虽然说常量不能在引用别的对象了，但是它的值如果是一个引用类型的话，引用对象的属性还是可以改的。
 const USER = {name:'terrt'};
 USER.name='112';
