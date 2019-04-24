# DevOps_Monkey
## 该monkey有多种模式使用
### 策略支持：

1. 模式 DFS
  --uiautomatordfs
  增加深度遍历算法

2. 模式 Mix 
--uiautomatormix
直接使用底层accessibiltyserver获取界面接口 解析各控件，随机选取一个控件执行touch操作。
  同时与原monkey 其他操作按比例混合使用
  默认accessibilityserver action占比50%，其余各action分剩余的50%
  accessibilityserver action占比可配置 --pct-uiautomatormix n

3. 模式Troy
  --uiautomatortroy
  控件选择策略按max.xpath.selector配置的高低优先级来进行深度遍历
