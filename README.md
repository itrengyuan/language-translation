# language-translate
用于将任意文件中的中文翻译成常见的语言，速度极快，翻译准确率极高。

## 基本用法
```
language-translation translate 文件路径
```
文件路径可以是绝对或者相对的路径，会默认将中文翻译成英语并生成一个新的文件。

## 指定翻译语言
```
language-translation translate 文件路径 对应语言的code
```
使用本行命令可以将文件翻译为指定语言。

## 如何查看支持翻译语言对应的code
```
language-translation lang
```
使用本行命令会得到所支持的语言的数据，如果想快速找到数据也可以使用：
```
   language-translation lang 对应语言的中文的首字发音的大写字母
```

例如输入 `language-translation lang Z` 会得到这样的格式。
``` js
[
    { name: '中文(简体)', code: 'zh' },
    { name: '中文(粤语)', code: 'yue' },
    { name: '中文(文言文)', code: 'wyw' },
    { name: '中文(繁体)', code: 'cht' }
]
```