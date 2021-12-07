长按规则编辑>查看子页面>断念插件调用>修改代码
```
items.push({    
title: '线路配置',    
url: "hiker://page/Route?rule=MyFieldᴰⁿ&type=设置#noHistory#", 

col_type: 'scroll_button'
});
items.push({    
title: '解析管理',    
url:"hiker://empty#noRecordHistory#@rule=js:this.d=[];$.require('hiker://page/jxItem?rule=MyFieldᴰⁿ').jxList();setResult(d)", 

col_type: 'scroll_button'
});
```
长按规则编辑>一级解析里，注释掉 const canUse=。。。 更换以下代码
```
var canUse=true;
```
