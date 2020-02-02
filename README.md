# vue-calendar-l 
vue日历组件
https://blog.csdn.net/qq_38188485/article/details/104134834

方法
select （选择日期）
monthChanged  （滑动移动月份）

传入参数：
| options  | type |  example | describe   |
| -------- | ---- | -------- | ---------- |
| options  | Object | { header_bg_color: "#ffffff", //头部颜色
        header_font_color: "#ffa300",//头部字体颜色
        week_font_color: "#333333", //星期字体颜色
        selected_bg_color: "#f49f19",//选择的背景颜色
        today_bg_color: "#f9d08f",//今天背景颜色
        event_dot_color: "#083ce4"//时间下面点的颜色 }  | 日历颜色 |
| value | Array | [“2019-02-01”]  | 默认选择日期   |
| begin | Array | [“2019-02-01”]  | 开始选择日期   |
| end | Array | [“2019-02-01”]  | 结束选择日期   |
| disabled | Array | [“2019-02-01”]  | 屏蔽的日期   |
| zero | Boolean | true  | 是否小于10补零   |
| weeks | Array | ["日", "一", "二", "三", "四", "五", "六"]  | 自定义星期名称  |
| months | Array | ["一月", "二月", "三月", "四月", "五月", "六月", "七月", "八月", "九月", "十月", "十一月", "十二月"]  | 自定义月份名称  |
| events | Array | [“2019-02-01-满”] | 自定义事件 （-最后是想要显示的字符  默认圆点）  |

npm包  npm install vue-calendar-l

在需要用到的页面中（注意 一个页面目前只能引入一次）

import Calendar from "vue-calendar-l";

components: { cTitle, cCalendar }

例子：

![图片说明](https://img-blog.csdnimg.cn/20200202111848163.png)

效果：

![图片说明](https://img-blog.csdnimg.cn/20200201155857217.gif)
