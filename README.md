# 灵工结算平台

#### 介绍
灵活用工结算开票平台，性能强劲稳定，久经市场考研，源码交付，支持SAAS架构。

#### 业务特点
- 支持多园区、多支付通道、多渠道
- 对接多银行、一键打包下载回单
- 发票自动在线申请
- 四要素认证
- 敏感词过滤
- 小程序在线手动签约
- 默认签约
- 银行回单一键下载
- 在线电子签约,支持君子签、E签宝、法大大
- 支付通道支持招商银行、平安银行、盛付通
- 支持在动申请下发电子发票

#### 联系
- 18297760325 微信同号
- 1030339985@qq.com 

#### 软件架构

- PHP实现WEB操作端，可以发挥PHP快速好用的特点；
- 使用NFS实现分布式文件共享；
- 使用JAVA SPRINGBOOT实现分布式结算处理服务、要素认证等功能，动态伸缩；
- 使用XXL-JOB实现任务的调度；
- 使用RabbitMQ实现队列以及服务的注册与发现。
- 相比于大厂的那些分布式微服务架构的庞大繁琐，该架构属于一种轻量级的自研架构，理解简单，极易部署。

#### 演示站点
- 网址：https://www.linggong.org.cn
- 用户名：demo
- 密码：abcd1234

#### 系统架构图
![avatar](https://gitee.com/wugu/lhyg/raw/master/assets/13.jpg)

#### 截图
![avatar](https://gitee.com/wugu/lhyg/raw/master/assets/1.jpg)
![avatar](https://gitee.com/wugu/lhyg/raw/master/assets/2.jpg)
![avatar](https://gitee.com/wugu/lhyg/raw/master/assets/3.jpg)
![avatar](https://gitee.com/wugu/lhyg/raw/master/assets/4.jpg)
![avatar](https://gitee.com/wugu/lhyg/raw/master/assets/5.jpg)
![avatar](https://gitee.com/wugu/lhyg/raw/master/assets/7.jpg)
![avatar](https://gitee.com/wugu/lhyg/raw/master/assets/8.jpg)
![avatar](https://gitee.com/wugu/lhyg/raw/master/assets/9.jpg)
![avatar](https://gitee.com/wugu/lhyg/raw/master/assets/10.jpg)
![avatar](https://gitee.com/wugu/lhyg/raw/master/assets/11.jpg)
![avatar](https://gitee.com/wugu/lhyg/raw/master/assets/12.jpg)



1. 业务流程：
![输入图片说明](https://gitee.com/wugu/lhyg/raw/master/assets/1.png)
2. 系统操作流程：
![输入图片说明](https://gitee.com/wugu/lhyg/raw/master/assets/22.jpg)
3. C端用户：
三、
- (一)用户注册

1. 姓名
2. 身份证号码
3. 实名手机号码
4. 身份证正反面上传
5. 开户行
6. 卡号

- (二)自然人实名认证

1. 企业方操作人截图保存弹框中签约二维码
2. 自然人微信扫描二维码，根据提示进行身份证拍照上传，并且绑定银行卡
3. 注意事项：
4. 1)同一自然人仅在首次发放时进行身份证上传步骤即可
5. 2)上传自然人的身份证有效期需大于2个月
6. 3)自然人需是年满18周岁不满75周岁的中国大陆居民，不支持港澳台及外籍人士发放
7. 4)不支持任何个体工商户经营者、做过税务登记者人员发放


- (三)用户登陆《微信授权登录或手机快捷登录(短信验证码登录)》
- (四)协议：《用户注册协议》、《用户隐私协议》、《服务协议》（无感）
- (五)绑定银行卡
- (六)接受任务（用户无感，登陆即确认接受任务）
- (七)任务列表明细（包括但不限于任务名称、接受任务日期、完成日期、结果金额、备注）
- (八)任务完成成果说明或相关资料上传
- (九)完税凭证下载(若有)
- 自然人可以在次月或次次月于“纳税申报”中查看下载完税资料
- (十)应用场景：电脑端或手机端（微信小程序、APP）


4. B端用户：
- (一)基本资料

1. 企业名称
2. 社会信用代码
3. 法定代表人
4. 法人身份证号码
5. 法人手机号码
6. 法人身份证正反面
7. 开户行
8. 银行账号

- (二)协议(合同档案)：

1. 《用户注册协议》
2. 《用户隐私协议》
3. 合同模版管理
4. 1)创建电子合同模板
5. 2)发起线上签订
6. 3)上传自然人与企业合同模板，

企业方操作人在“合同模板”中点击【上传纸质合同模板】，自定义模板名称（如有多份合同模板，请注意区分）；选择对应甲方、职业类型；模板详情处 需将Word合同模板的全部内容复制粘贴；点击【确认】即可

1. 4)上传已签署的合同扫描版
若线下与自然人签订业务合作协议并盖章，扫描成pdf、jpg、png格式；在“合同档案”中，点击【上传纸质合同】，可选择单个上传或批量上传
- (三)任务管理

1. 1.任务名称
1. 2.任务类型
1. 3.任务地点
1. 4.结算方式
1. 5.结算金额

注意：系统设置为单人单日/单月发放金额不得低于****元，不超过**万元

- (四)订单管理（项目包括但不限于：发布任务时间、任务名称、发布任务公司、姓名、账户名、结算金额、结算时间、结算状态、备注）
- (五)款项明细表（包括期初余额、本期充值金额、本期发放金额、期末金额）
- (六)开票管理

1. 企业方操作人在“发票申请”中点击【申请发票】，勾选需要开票的账单进行申请（按一个订单开票或多个订单汇总）
2. 注意：系统设置为单张发票金额不得超过10万元
3. 发票自动下载
4. 开票记录

- (七)完税凭证下载(若有)
企业方操作人可以在次月或次次月于“纳税申报”中查看下载完税资料
- (八)银行回单管理

1. 系统按结算详情自动从第三方支付抓取付款回单上传
2. 一键下载回单


- (九)账户日记
- (十)应用场景：电脑端或手机端（微信小程序、APP）


1. 5. 平台端


- (一)查询统计功能（按期间、企业名称、个人用户名、发票开具状态等）
- (二)导入导出Excel功能
- (三)后台审核功能
- (四)完税凭证资料自动上传(若有)
- (五)用户操作权限授权管理功能



1. 6. 数据接口：

- (一)款项支付接口（盛付通支付或银行接口）
- (二)发票接口（税务系统或第三方代理商）
- (三)完税凭证接口（税务系统或第三方代理商）
- (四)企业信息接口（工商系统或第三方代理商）
- (五)个人身份证接口（公安系统或第三方代理商）

在线电子签名接口（小程序在线签名

1. 7. 其他功能

- (一)发票在线自动申请、发票批量上传及下载
- (二)银行回单一键打包下载
- (三)查询功能做配置
- (四)合同档案管理(导入导出功能，支持pdf、jpg、png格式)
- (五)纳税申报管理(企业方操作人可以在次月或次次月于“纳税申报”中查看下载完税资料)


