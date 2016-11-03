---
title: mysql length
date: 2016-11-03 17:40:11
categories: mysql
tags:
---

转载自: http://yishouce.com/mysql/func/length

一句话说明: 获取字符串长度的mysql内置函数

length是mysql的一个用来来获取字符串长度的内置函数方法, 同样的获取字符串长度的还有char_length. length: 是计算字段的长度, utf8编码下,一个汉字是算三个字符,一个数字或字母算一个字符。其他编码下,一个汉字算两个字符, 一个数字或字母算一个字符。

例子1: 查看mysql字符串的长度

    SELECT LENGTH("要查看长度的mysql字段/mysql字符串");

例子2: 根据记录的某个字段长度排序

    SELECT * FROM table WHERE 1 ORDER BY LENGTH(name) ASC;

相关: char_length:在任何编码下, 不管汉字还是数字或者是字母都算是一个字符. CHARACTER_LENGTH(str) CHARACTER_LENGTH()是CHAR_LENGTH()的同义词。 BIT_LENGTH(str) 返回2进制长度.
