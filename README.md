网站流量统计系统-数据分析模块
========================


### 日志数据分析模块注意事项
+ 按特定规则分集合存储，比如有些URL被归为PC端，有些被归为移动端，有些被归为第三方合作等等；
+ 按自然日期时间分时归档存储，按时、日、周、月以不同集合存储，存储结构尽量保持一致；
+ 分析结果集合不设置检索字段，如来源类型、设备类型、地域、新老访客等等；



趋势 trend

    site * uv pv ip 新访客数 直接访问数 搜索引擎来源数 外部链接 桌面电脑数 手机设备数 平板数
    小时 date hour
    日 date
    周 Y week
    月 Ym

trend_hour
trend_day
trend_week
trend_month

下同

搜索引擎 searchengine

    site * {main_searchengine} {sub_searchengine} uv pv ip 新访客数 搜索引擎数 桌面电脑数 手机设备数 平板数
    小时 date hour
    日 date
    周 Y weed
    月 Ym

搜索词 searchword

    site * {word} uv pv ip 新访客数 桌面电脑数 手机设备数 平板数
    小时 date hour
    日 date
    周 Y weed
    月 Ym

外部链接 referrer 仅记录最多的前200个具体的连接，其余部分全部归为其他来源

    site * {ref} uv pv ip 新访客数 桌面电脑数 手机设备数 平板数
    小时 date hour
    日 date
    周 Y weed
    月 Ym

受访页面 access_page 仅记录最多的前500个具体的连接，其余部分全部归为其他来源

    site * {url} uv pv ip 新访客数 直接访问数 搜索引擎来源数 外部链接 桌面电脑数 手机设备数 平板数
    小时 date hour
    日 date
    周 Y weed
    月 Ym

受访域名 access_domain

    site * {domain} uv pv ip 新访客数 直接访问数 搜索引擎来源数 外部链接 桌面电脑数 手机设备数 平板数
    小时 date hour
    日 date
    周 Y weed
    月 Ym

地域分析 region

    site * {region} uv pv ip 新访客数 直接访问数 搜索引擎来源数 外部链接 桌面电脑数 手机设备数 平板数
    小时 date hour
    日 date
    周 Y weed
    月 Ym

系统环境 - 设备厂商 vendor/设备类型 type/设备型号 model/浏览器 browser/网络服务网商 isp

    site * {设备类型/设备型号/浏览器/网络服务网商} uv pv ip
    小时 date hour
    日 date
    周 Y weed
    月 Ym

新老访客 visitor

    site * {新老访客} uv pv ip 直接访问数 搜索引擎来源数 外部链接 桌面电脑数 手机设备数 平板数
    小时 date hour
    日 date
    周 Y weed
    月 Ym
