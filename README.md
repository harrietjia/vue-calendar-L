# vue-calendar-l 
vue日历组件
https://blog.csdn.net/qq_38188485/article/details/104134834

方法
select （选择日期）
monthChanged  （滑动移动月份）

传入参数：

  options: {
    type: Object,
    default: function() {
      return {
        header_bg_color: "#ffffff", //头部颜色
        header_font_color: "#ffa300",//头部字体颜色
        week_font_color: "#333333", //星期字体颜色
        selected_bg_color: "#f49f19",//选择的背景颜色
        today_bg_color: "#f9d08f",//今天背景颜色
        event_dot_color: "#083ce4"//时间下面点的颜色
      };
    }
  },
  // 默认选择日期  日期格式传入[“2019-02-01”]
  value: {
    type: Array,
    default: function() {
      return [];
    }
  },
  // 开始选择日期
  begin: {
    type: Array,
    default: function() {
      return [];
    }
  },
  // 结束选择日期
  end: {
    type: Array,
    default: function() {
      return [];
    }
  },
  // 是否小于10补零
  zero: {
    type: Boolean,
    default: true
  },
  // 屏蔽的日期
  disabled: {
    type: Array,
    default: function() {
      return [];
    }
  },
  // 是否显示农历
  lunar: {
    type: Boolean,
    default: false
  },

  // 自定义星期名称
  weeks: {
    type: Array,
    default: function() {
      return window.navigator.language.toLowerCase() == "zh-cn" ? ["日", "一", "二", "三", "四", "五", "六"] : ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"];
    }
  },
  // 自定义月份名称
  months: {
    type: Array,
    default: function() {
      return window.navigator.language.toLowerCase() == "zh-cn" ? ["一月", "二月", "三月", "四月", "五月", "六月", "七月", "八月", "九月", "十月", "十一月", "十二月"] : ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"];
    }
  },
  // 自定义事件  日期格式传入[“2019-02-01-满”]  最后是想要显示的字符  默认圆点
  events: {
    type: Array,
    default: function() {
      return [];
    }
  }

npm包  npm install vue-calendar-l

在需要用到的页面中（注意 一个页面目前只能引入一次）

import Calendar from "vue-calendar-l";

components: { cTitle, cCalendar }

例子：

![图片说明](https://img-blog.csdnimg.cn/20200202111848163.png)

效果：

![图片说明](https://img-blog.csdnimg.cn/20200201155857217.gif)
