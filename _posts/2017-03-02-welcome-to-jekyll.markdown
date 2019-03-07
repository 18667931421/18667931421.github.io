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
 
 //es6新增加的二种声明变量的方式，可以解决var以前的一些问题。
 
 三、解构
 解构即是 分解一个对象的结构
 
 let arr =[1,2,3];
 lat a=arr[0];
 // 解构的时候，等号两边的结构类似。右边还必须是一个真实的值
 let [a,b,c] = arr;
 
 let obj = {name:'zfpx',age:9}
 let {name:myname, age:myage} = obj;
 => let myname = obj.name
 
 默认解构 如果能取出来的值就用取出来的值，如果取不出来就用默认值
 let obj2 = {name:'zfd'}
 let {name,age=8} = obj2;
 
 
 
 