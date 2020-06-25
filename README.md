# wmms项目接口说明

## 一、接口更新日志

### 2020-06-25

#### 1.系统菜单管理

（1）、菜单的新增、获取、删除、更新、列表查询接口如下图所示。特别说明，菜单没有上级时传，字段“parentId”传“-1”。
      ![](https://cdn.jsdelivr.net/gh/lixinyuan1213/wmms_dashboard@master/images/menu1.jpg)



（2）、**根据登录人角色获取，菜单，用于菜单展示。已经处理成了树状结构。**  特别说明，超级管理员会获取所有的菜单。name 不用传。当前很多菜单没有录入。

![](https://cdn.jsdelivr.net/gh/lixinyuan1213/wmms_dashboard@master/images/menu2.jpg)



#### 2. 角色和菜单绑定

（0）、操作步骤，应该在“系统管理”-“角色管理”后面添加一个“绑定菜单“的按钮，点击后以树形结构显示菜单，

选择对应的菜单，完成添加和修改。

![](https://cdn.jsdelivr.net/gh/lixinyuan1213/wmms_dashboard@master/images/menu5.jpg)

参考：

![](https://cdn.jsdelivr.net/gh/lixinyuan1213/wmms_dashboard@master/images/menu6.jpg)

（1）、角色和菜单的绑定、修改接口。整合操作需要结合（2）的接口

![](https://cdn.jsdelivr.net/gh/lixinyuan1213/wmms_dashboard@master/images/menu3.jpg)

（2）、根据角色id获取菜单接口

![](https://cdn.jsdelivr.net/gh/lixinyuan1213/wmms_dashboard@master/images/menu4.jpg)

### 2020-06-23

#### 首页统计

1. 按照月/季度获取平台（或者个人）用水量

      ![](https://cdn.jsdelivr.net/gh/lixinyuan1213/wmms_dashboard@master/images/readermonth.jpg)

      对应：
      ![](https://cdn.jsdelivr.net/gh/lixinyuan1213/wmms_dashboard@master/images/dui1.jpg)
      
2. 按照月/季度获取平台（或者个人）缴费情况
      ![](https://cdn.jsdelivr.net/gh/lixinyuan1213/wmms_dashboard@master/images/paymonth.jpg)
 对应：
      ![](https://cdn.jsdelivr.net/gh/lixinyuan1213/wmms_dashboard@master/images/dui1.jpg)

3. 一次性获取平台（或者个人）用月/季度水量和缴费情况
      ![](https://cdn.jsdelivr.net/gh/lixinyuan1213/wmms_dashboard@master/images/alls.jpg)

       对应：
      ![](https://cdn.jsdelivr.net/gh/lixinyuan1213/wmms_dashboard@master/images/dui1.jpg)
      
4. 一次性获取首页的统计信息（用户总数、设备总数、抄表次数、支付次数、支付总额、用水总数）
    ![](https://cdn.jsdelivr.net/gh/lixinyuan1213/wmms_dashboard@master/images/zonghe.jpg)

    对应：

    ![](https://cdn.jsdelivr.net/gh/lixinyuan1213/wmms_dashboard@master/images/dui2.jpg)

5. 各自获取用户总数、设备总数、抄表次数、支付次数、支付总额、用水总数
    ![](https://cdn.jsdelivr.net/gh/lixinyuan1213/wmms_dashboard@master/images/youall.jpg)

### 2020-06-22

1. 新增remark（可以为空。不为空时，最少字数为1，最大为200）字段

   ![](https://cdn.jsdelivr.net/gh/lixinyuan1213/wmms_dashboard@master/images/remark.jpg)

2. 缴费时新增缴费方式字段。

    ![](https://cdn.jsdelivr.net/gh/lixinyuan1213/wmms_dashboard@master/images/payment.jpg)

## 二、功能实现

1. 计算水费