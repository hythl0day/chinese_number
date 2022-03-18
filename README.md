# Chinese number parser & converter

Convert **integer** numbers from Chinese character to Dart integer.
Convert Dart integer & double values to Chinese character.

## Usage

```dart
final str = '拾壹万叁仟肆佰贰拾壹';
print(ChineseNumber.tryParse(str));

final n = 214323232003;
print(n.toSimplifiedChineseNumber());
print(n.toFormalSimplifiedChineseNumber());
print(n.toTraditionalChineseNumber());
```

## About

This package is derived from Anton Ivanov's Javascript code:
https://github.com/anton-bot/chinese-numbers-converter.js
We re-written the code in Dart and removed some useless part.
And Hans Yang's Dart code:
https://pub.dev/packages/number_to_chinese
We extended his code to Simplified Chinese.
