---
title: JS逆向(1)-笑亖，根本不用开VIP
description: sojson版本检测与防格式化原理
author: VeryrrDefine
date: 2025-1-18 23:50:00 +0800
categories: [Blog]
tags: [逆向, js]
pin: true
math: true
mermaid: true
image:
  path: /assets/img/user/202501051.png
---

sojson网站有一个加密工具(https://www.sojson.com/jsobfuscator.html),内有"防止格式化选项"，另外还有"jsjiami.com.v5 不能去掉"
接下来我会揭示它们的原理


```javascript 
//SOJSON内置示例代码
var a={},b={}; 

(function(w, d) { 

 w.info = "这是一个一系列js操作。"; 

 d.warning = "如果您的JS里嵌套了PHP，JSP标签，等等其他非JavaScript的代码，请提取出来再加密。这个工具不能加密php、jsp等模版内容"; 

 d.intro = "本工具由 www.jsjiami.com 提供接口。"; 

})(a, b);
```

首先，加密；加密以后是这个样子

```javascript
/*
 * 加密工具已经升级了一个版本，目前为 jsjiami.com.v5 ，主要加强了算法，以及防破解【绝对不可逆】配置，耶稣也无法100%还原，我说的。;
 * 已经打算把这个工具基础功能一直免费下去。还希望支持我。
 * 另外 jsjiami.com.v5 已经强制加入校验，注释可以去掉，但是 jsjiami.com.v5 不能去掉（如果你开通了VIP，可以手动去掉），其他都没有任何绑定。
 * 誓死不会加入任何后门，jsjiami.com JS 加密的使命就是为了保护你们的Javascript 。
 * 警告：如果您恶意去掉 jsjiami.com.v5 那么我们将不会保护您的JavaScript代码。请遵守规则
 * 新版本: https://www.jsjiami.com/ 支持批量加密，支持大文件加密，拥有更多加密。 */
 
;var encode_version = 'jsjiami.com.v5', foeoz = '__0x123597',  __0x123597=['TUtOcWM=','c09IUEc=','5Yig6Zmk54mI5pys5Y+377yManPkvJrlrprmnJ/lvLnnqpc=','6L+Z5piv5LiA5Liq5LiA57O75YiXanPmk43kvZzjgII=','5pys5bel5YW355SxIHd3dy5qc2ppYW1pLmNvbSDmj5DkvpvmjqXlj6PjgII=','R2JHd3U=','d2FybmluZw==','5aaC5p6c5oKo55qESlPph4zltYzlpZfkuoZQSFDvvIxKU1DmoIfnrb7vvIznrYnnrYnlhbbku5bpnZ5KYXZhU2NyaXB055qE5Luj56CB77yM6K+35o+Q5Y+W5Ye65p2l5YaN5Yqg5a+G44CC6L+Z5Liq5bel5YW35LiN6IO95Yqg5a+GcGhw44CBanNw562J5qih54mI5YaF5a65','aW50cm8=','QkZmd3E=','anNqaWFtaS5jb20udjU=','54mI5pys5Y+377yManPkvJrlrprmnJ/lvLnnqpfvvIzov5jor7fmlK/mjIHmiJHku6znmoTlt6XkvZw='];(function(_0x429b84,_0xea203e){var _0x5869d6=function(_0x1a934e){while(--_0x1a934e){_0x429b84['push'](_0x429b84['shift']());}};_0x5869d6(++_0xea203e);}(__0x123597,0x123));var _0x5442=function(_0x58268d,_0x60b92e){_0x58268d=_0x58268d-0x0;var _0x10efad=__0x123597[_0x58268d];if(_0x5442['initialized']===undefined){(function(){var _0x520b2a=typeof window!=='undefined'?window:typeof process==='object'&&typeof require==='function'&&typeof global==='object'?global:this;var _0x1ae5c9='ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/=';_0x520b2a['atob']||(_0x520b2a['atob']=function(_0x6f6693){var _0x29df45=String(_0x6f6693)['replace'](/=+$/,'');for(var _0x4ec641=0x0,_0x46a275,_0x22de4f,_0x44ccf6=0x0,_0x24a78e='';_0x22de4f=_0x29df45['charAt'](_0x44ccf6++);~_0x22de4f&&(_0x46a275=_0x4ec641%0x4?_0x46a275*0x40+_0x22de4f:_0x22de4f,_0x4ec641++%0x4)?_0x24a78e+=String['fromCharCode'](0xff&_0x46a275>>(-0x2*_0x4ec641&0x6)):0x0){_0x22de4f=_0x1ae5c9['indexOf'](_0x22de4f);}return _0x24a78e;});}());_0x5442['base64DecodeUnicode']=function(_0xf3d5e4){var _0x33b476=atob(_0xf3d5e4);var _0x45c047=[];for(var _0x19f352=0x0,_0x463f2b=_0x33b476['length'];_0x19f352<_0x463f2b;_0x19f352++){_0x45c047+='%'+('00'+_0x33b476['charCodeAt'](_0x19f352)['toString'](0x10))['slice'](-0x2);}return decodeURIComponent(_0x45c047);};_0x5442['data']={};_0x5442['initialized']=!![];}var _0x2a859c=_0x5442['data'][_0x58268d];if(_0x2a859c===undefined){_0x10efad=_0x5442['base64DecodeUnicode'](_0x10efad);_0x5442['data'][_0x58268d]=_0x10efad;}else{_0x10efad=_0x2a859c;}return _0x10efad;};var a={},b={};(function(_0x180581,_0x4ed433){var _0x3f2010={'GbGwu':_0x5442('0x0'),'BFfwq':_0x5442('0x1')};_0x180581['info']=_0x3f2010[_0x5442('0x2')];_0x4ed433[_0x5442('0x3')]=_0x5442('0x4');_0x4ed433[_0x5442('0x5')]=_0x3f2010[_0x5442('0x6')];}(a,b));;(function(_0x225e54,_0x3d8761,_0x437836){var _0x343665={'xRXHo':'ert','MKNqc':'undefined','pCQfN':function _0x199a96(_0x2a06c2,_0x142fd7){return _0x2a06c2===_0x142fd7;},'EVZNu':_0x5442('0x7'),'sOHPG':function _0x1004f1(_0x54faf7,_0x38b885){return _0x54faf7+_0x38b885;},'tbbjp':_0x5442('0x8')};_0x437836='al';try{_0x437836+=_0x343665['xRXHo'];_0x3d8761=encode_version;if(!(typeof _0x3d8761!==_0x343665[_0x5442('0x9')]&&_0x343665['pCQfN'](_0x3d8761,_0x343665['EVZNu']))){_0x225e54[_0x437836](_0x343665[_0x5442('0xa')]('删除',_0x343665['tbbjp']));}}catch(_0x242408){_0x225e54[_0x437836](_0x5442('0xb'));}}(window));;encode_version = 'jsjiami.com.v5';
```

乍一看，前面有个`__0x123597`变量，扔进node里，然后`__0x123597.map((x)=>atob(x))`，得出以下结果: 
```javascript
[
  'MKNqc',
  'sOHPG',
  atob('5Yig6Zmk54mI5pys5Y+377yManPkvJrlrprmnJ/lvLnnqpc='),
  atob('6L+Z5piv5LiA5Liq5LiA57O75YiXanPmk43kvZzjgII='),
  atob('5pys5bel5YW355SxIHd3dy5qc2ppYW1pLmNvbSDmj5DkvpvmjqXlj6PjgII='),
  'GbGwu',
  'warning',
  atob('5aaC5p6c5oKo55qESlPph4zltYzlpZfkuoZQSFDvvIxKU1DmoIfnrb7vvIznrYnnrYnlhbbku5bpnZ5KYXZhU2NyaXB055qE5Luj56CB77yM6K+35o+Q5Y+W5Ye65p2l5YaN5Yqg5a+G44CC6L+Z5Liq5bel5YW35LiN6IO95Yqg5a+GcGhw44CBanNw562J5qih54mI5YaF5a65'),
  'intro',
  'BFfwq',
  'jsjiami.com.v5',
  atob('54mI5pys5Y+377yManPkvJrlrprmnJ/lvLnnqpfvvIzov5jor7fmlK/mjIHmiJHku6znmoTlt6XkvZw=')  
]
```
部分字符串解码出乱码，但放在base64.us解密就可以得到
```javascript
[
  'MKNqc',
  'sOHPG',
  '删除版本号，js会定期弹窗',
  '这是一个一系列js操作。',
  '本工具由 www.jsjiami.com 提供接口。',
  'GbGwu',
  'warning',
  '如果您的JS里嵌套了PHP，JSP标签，等等其他非JavaScript的代码，请提取出来再加密。这个工具不能加密php、jsp等模版内容',
  'intro',
  'BFfwq',
  'jsjiami.com.v5',
  '版本号，js会定期弹窗，还请支持我们的工作'  
]
```

# 版本号？

## 分析
可以发现两个版本号内容，一看就是版本号检测。

有的人问了，删除了**版本号**会怎么样？

首先注入alert，这一步的目的是为了看**调用堆栈**。

```javascript 
originalAlert = alert;
alert = function(x){
  console.log(x);
  debugger;
}
```

删除版本号后，运行

可以看到顺利触发debugger了:
![/assets/img/user/015f829676ff74911cd950ff6aff5eca.png](/assets/img/user/015f829676ff74911cd950ff6aff5eca.png)

可以发现，后面的**try catch**代码起到了关键作用。

版本号弹窗解决方法很简单。直接把后面的**try catch**代码删除就解决了。
```javascript 
try{_0x437836+=_0x343665['xRXHo'];_0x3d8761=encode_version;if(!(typeof _0x3d8761!==_0x343665[_0x5442('0x9')]&&_0x343665['pCQfN'](_0x3d8761,_0x343665['EVZNu']))){_0x225e54[_0x437836](_0x343665[_0x5442('0xa')]('删除',_0x343665['tbbjp']));}}catch(_0x242408){_0x225e54[_0x437836](_0x5442('0xb'));}
```
## 原理
实际上就是检测`encode_version`存不存在，然后弹窗。


# 格式化检测
没找到，以后再说
