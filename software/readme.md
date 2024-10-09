# 软件设计

## 一、整体架构
![图片1](/images/01_software_framework.png)


## 二、系统模块功能
### 2.1 微信小程序
小程序通过微信扫码登录，分为教师和家长两种模式  
教师模式主要负责学生的测量，学生数据由后台统一维护  
家长可以自行添加小孩信息，进行每日测量及历史数据观察

![图片2](/images/02_wechat_app.png)

### 2.2 后台服务

后端服务主要提供数据管理功能，可以对教师和学生信息进行批量录入  
通过对接第三方的健康数据接口，结合脊柱测量信息进行健康评估和分析  
支持生成历史趋势数据，并支持自定义报表  

![图片3](/images/03_server.png)

## 三、数据模型
### 2.1 对象模型

#### ts_user 用户信息表
![图片4](/images/04_ts_user.png)

#### tr_user_student 用户所属学生表

![图片5](/images/05_ts_user_student.png)

#### tr_student_measure 学生测量记录表

![图片6](/images/06_student_measure.png)


#### ts_user_dev 用户绑定信息
![图片7](/images/07_user_dev.png)


#### ts_app_material app素材管理
![图片8](/images/08_app_material.png)


#### ts_upload_info 上传文件信息管理
![图片9](/images/09_ts_upload_info.png)

## 四、界面展示

备注：以下为真实测试案例，已去掉隐私信息

![图片10-a](/images/10_show_a.png)


![图片10-b](/images/10_show_b.png)

![图片10-c](/images/10_show_c.png)
