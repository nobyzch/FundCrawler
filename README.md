# 天天基金爬虫
爬取天天基金网，辅助对基金投资的选择

## 功能特性
- 爬取天天基金网上所有的基金，及相应基金经理，以往的收益率等

- 模仿tcp的拥塞控制的反爬控制，线程数量，慢开始，拥塞避免
- 爬取全部数据需要470s（不使用代理），瓶颈为网站的反爬策略
- 留有从文件中批量导入代理ip的代码，理论上可大大提升爬取效率（需简单修改代码）
    - 爬取免费代理的脚本在另一个profile，crawler_tools，爬取的对象为西刺所提供的免费代理ip
    - 由于免费代理ip非常不稳定，大概率会导致比原本更慢的情况

## 以后的更新
- 重构
- bug修复，有几个基金在重复爬取后仍然失败，基金总数有缺失
- 数据可视化
