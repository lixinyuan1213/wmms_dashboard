# wmms项目接口说明

## 一、接口更新日志

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