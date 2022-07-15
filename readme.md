### 这是Linux基础课的thrift教学项目

#### 作者简介
我是王思哲，嗨嗨嗨！

#### 内容简介
这个项目实现了一个游戏匹配系统：
    1. game_client端发送添加/删除用户的请求
    2. match_system的match端处理请求
    3. match_system的save端发送保存数据的请求给远程服务器ACS_5715,实现数据保存。


#### 功能特色
    1. 实现了匹配时的多线程处理技术
    2. 根据用户等待时间不断扩大该用户的匹配池（根据分数匹配）

#### thrift接口介绍
两个接口，分别实现 匹配 & 保存数据（返回匹配结果）功能
    1. Match接口
       定义User结构体，确定传递数据类型。
       定义Service：add_user & remove_user
    2. Save接口
       定义Servive：Save
