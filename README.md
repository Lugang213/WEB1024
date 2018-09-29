## 胜天半子的前端博客

  谷地平整四方如棋盘，黑石白雪间隔如棋子，恰成一局围棋。教师思忖许久，方猜出浑沌冻死前搬石取暖，无意中摆出这局棋。真是棋痴!再细观此局，但见构思奇特，着数精妙，出磅礴大气，显宇宙恢宏，实在是他生平未见的伟大作品。群山巍峨，环棋盘而立;长天苍苍，垂浓云而下;又有雄鹰盘旋山涧，长啸凄厉……
  官屯教师身心震动，肃穆久立。
  众人登山围拢教师，见他异样神情皆不解。纷纷问道：“你看什么?浑沌干啥?”教师答：“下棋。”“深山旷野，与谁下棋?”教师沉默不语。良久，沉甸甸道出一字：“天!”
  俗人浅见，喳喳追问：“赢了还是输了?”
  教师细细数目。数至右下角，见到那个决定胜负的劫。浑沌长跪于地，充当一枚黑子，恰恰劫胜!教师崇敬浑沌精神，激情澎湃。他双手握拳冲天高举，喊得山野震荡，林木悚然——
  “胜天半子!”

### H5全栈工程师

全栈工程师是指掌握多种技能，并能利用多种技能独立完成产品的人。 [1]  也叫全端工程师(同时具备前端和后台能力)，英文Full Stack engineer。

```markdown
前端工程师

# JavaScript
## HTML5+CSS3
### Node.js

- Node.js+Express+MongoDB搭建个人博客
- Vue.js+Webpack生成移动端项目

1. 微信小程序
2. 微信公众号

**AJAX** 异步的JavaScript和XML

[Link](url) and ![Image](src)
```

欢迎访问 [小白猿个人博客](http://www.luggang.com).

### 什么是 AJAX ？

AJAX = 异步 JavaScript 和 XML。
AJAX 是一种用于创建快速动态网页的技术。
通过在后台与服务器进行少量数据交换，AJAX 可以使网页实现异步更新。这意味着可以在不重新加载整个网页的情况下，对网页的某部分进行更新。
传统的网页（不使用 AJAX）如果需要更新内容，必需重载整个网页面。
有很多使用 AJAX 的应用程序案例：新浪微博、Google 地图、开心网等等。

### 原生AJAX
```markdown
  function Ajax(obj){
    //根据obj对method,data,url等进行初始化
  };
  Ajax.prototype.send = function(){
    var xhr = new XMLHttpRequest();//新建ajax请求，不兼容IE7以下
    xhr.onreadystatechange = function(){//注册回调函数
      if(xhr.readyState === 4)
        callback(xhr.responseText);
    }
    if(method === 'get'){//如果是get方法，需要把data中的数据转化作为url传递给服务器
      xhr.open(method,url,true);
      xhr.send(null);
    }else if(method === 'post'){//如果是post，需要在头中添加content-type说明
        xhr.open(method,url,true);
        xhr.setRequestHeader('Content-Type','application/x-www-form-urlencoded');
        xhr.send(JSON.stringify(data));//发送的数据需要转化成JSON格式
    }else {
      console.log('不识别的方法:'+method);
      return fasle;
    }
  }
```

