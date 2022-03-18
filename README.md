# 中文数字转换

- 将汉字字符串形式的数字（**仅限整数**）转换为 Dart 的 int 值。

- 将 Dart 中的整数或者浮点数转换为汉字字符串。

## 使用方法

```dart
final str = '拾壹万叁仟肆佰贰拾壹';
print(ChineseNumber.tryParse(str)); // 113421

final n = 214323232003;
print(n.toSimplifiedChineseNumber()); // 二千一百四十三亿二千三百二十三万二千零三
print(n.toFormalSimplifiedChineseNumber()); // 贰仟壹佰肆拾叁亿贰仟叁佰贰拾叁万贰仟零叁
print(n.toTraditionalChineseNumber()); // 貳仟壹佰肆拾叁億貳仟叁佰貳拾叁萬貳仟零叁
```

## 关于代码

这个包参考了 Anton Ivanov 的 Javascript 代码：
https://github.com/anton-bot/chinese-numbers-converter.js
我们将其用 Dart 重写，但去掉了一些和本项目无关的内容。

也参考了 Hans Yang 的另一个汉字数字转换包：
https://pub.dev/packages/number_to_chinese
但我们将其扩展为可以支持简体中文汉字。

# Chinese number parser & converter

- Convert **integer** numbers from Chinese character to Dart integer.

- Convert Dart integer & double values to Chinese character.

## Usage

```dart
final str = '拾壹万叁仟肆佰贰拾壹';
print(ChineseNumber.tryParse(str)); // 113421

final n = 214323232003;
print(n.toSimplifiedChineseNumber()); // 二千一百四十三亿二千三百二十三万二千零三
print(n.toFormalSimplifiedChineseNumber()); // 贰仟壹佰肆拾叁亿贰仟叁佰贰拾叁万贰仟零叁
print(n.toTraditionalChineseNumber()); // 貳仟壹佰肆拾叁億貳仟叁佰貳拾叁萬貳仟零叁
```

## About

This package is derived from Anton Ivanov's Javascript code:
https://github.com/anton-bot/chinese-numbers-converter.js
We re-written the code in Dart and removed some useless part.

And Hans Yang's Dart code:
https://pub.dev/packages/number_to_chinese
We extended his code to Simplified Chinese.
