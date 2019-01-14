# jsDoc
规范注释，学习jsDoc

## 常用注释

    @author 作者
    @class @constructor  标记类 构造函数
    @description  @desc  描述
    @module 模块名称
    @enum   枚举类型标记
    @global 全局对象标记
    @param  函数参数标记
    @returns @return 函数返回标记
    @this   this指向标记
    @memberof   模块间从属关系标记
    @event 在模块中标记 可以被触发的事件  与 @fire 配合使用

## demo

```js
/**
 * 测试注释
 * @method addEvent
 * @description 绑定事件的方法
 * @param  {String}     ele         要添加时间的
 * @param  {String}     type        事件类型
 * @param  {Function}   callBack    回调函数
 * @return {Boolean}               返回值
 */
function addEvent(ele,type,callBack){
    document.getElementById(ele).addEventListener(type,callBack);
    return true;
}
```

    暂时先以这种方式写备注,要生成文档需要node配合。