# datetime-picker
移动端时间日期控件
![日期](https://github.com/vue-tools/vt-datetime-picker/img/date.png)
![时间](https://github.com/vue-tools/vt-datetime-picker/img/time.png)

# Use
```shell
$ npm install vt-datetime-picker -s
```

```shell
 import datetimePicker from 'vt-datetime-picker'
 
 Vue.component('DatetimePicker', datetimePicker)
```
 # ependent
 
该组件依赖[vt-picker](https://github.com/vue-tools/vt-picker)组件
 
 # Api
 ### Props 
*   `value` String类型，默认选中的值，可以是空字符串，**更改该属性，组件立刻更新**
*   `type` 时间日期的输出类型，如 `yyyy-MM-dd hh:mm:ss`,分隔字符支持自定义
    - yyyy:年份
    - MM:月份
    - dd:天数
    - hh:小时（24小时制）
    - mm:分钟数
    - ss:秒数
*   `max` 能选择最大日期，默认`2099-12-31`

# Waring
* 该组件必须有v-model指令，否则会发生错误
* `type`属性 `年` `月` `日`  `时` `分` `秒` 必须是连续的，不支持如`yyyy-MM hh:mm`这种格式
