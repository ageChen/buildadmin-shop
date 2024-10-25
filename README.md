# 介绍

基于 `BuildAdmin` 和 `Uni-app` 的商城应用。

服务端支持 `常驻内存运行` ，客户端支持编译为 `微信小程序` 和 `H5网页` 。



# 项目主页

点击访问项目主页：[JoyShop商城](https://modules.buildadmin.com/joyshop)



# 技术栈

后端： `thinkPHP8 ` + `MySQL8` +`redis` + `easyWechat` + `yansongda/pay `  等

前端： `vue3` + `typescript` + `uniapp`  等



# 功能特性

## 控制台

以直观清晰的布局，全面展示商城如订单销售量、销售额、用户注册数量以及周期同比增长率等关键数据，让您如同拥有商城运营的“全景地图”，轻松把握运营态势和趋势。 



## 广告位管理

灵活设置前台轮播图、滚动公告栏 和 商品橱窗。 

支持设置轮播图和商品橱窗快速跳转详情或列表。



## 商品管理

支持灵活设置商品规格信息，商品库存扣减方式，初始销量等。

支持 `折叠` 展示商品规格信息，快捷上下架商品等操作。



## 模板填充

支持对商品规格、商品参数、商家服务与承诺等 `配置模板` ，在添加和编辑时实现快速填充。



## 库存预警

支持对商品和规格分别设置库存预警值，对库存不足的商品及时在页面 `高亮预警` 。

支持列表页快速补充库存，轻松应对库存变化。



## 订单管理

支持快速筛查不同订单状态，对订单待处理状态以徽标显著提醒。

提供订单状态变更时间记录和变更日志追踪，及时把握整个订单流程。



## 订单发货

支持 `统一发货` 和 `分拆发货` ，满足不同发货需求。

已接入 [小程序发货信息管理](https://developers.weixin.qq.com/miniprogram/product/jiaoyilei/fahuoguanligongneng.html) 和 [小程序确认收货组件](https://developers.weixin.qq.com/miniprogram/dev/platform-capabilities/business-capabilities/order-shipping/order-shipping-half.html)，无需手动到小程序后台输入物流信息。



## 订单导出

采用 `异步队列` 方案实现订单导出，支持处理 `大数据量 `。

支持 `按页面搜索条件` 和 `按字段` 自定义导出，满足多样化的数据分析需求。



## 订单售后

具备完善的订单售后功能，为用户提供优质、便捷的订单服务，提升用户的购物体验和满意度。 



## 订单评价

用户可通过订单对商品进行评价，后台可查看和管理商品评价。 不仅为用户提供了表达意见和反馈的渠道，也有助于了解用户的需求和意见，从而不断改进和优化商品及服务。



## 物流管理

轻松设置售后物流地址信息，方便管理物流快递公司。

支持 `自定义运费模板`，根据不同地区，按件数、重量、体积等因素灵活设置运费规则，实现物流成本的精准控制。 



## 优惠券模块

支持设置 `满减券` 和 `折扣券` ，自定义优惠券类型 ，可通过领券中心设置优惠券发放，查看用户领券情况。



## 充值中心

充值中心支持 `自定义套餐` 充值金额与赠送金额，增加用户预充值意愿，提高资金流动性 。



## 物流追踪

对接 `微信小程序物流组件` 和 `快递100` 物流查询服务商，满足多种物流查询需求。



## 商城配置

按照功能模块对商城的配置项进行清晰分组，提供便捷、高效的操作界面。

支持`快速添加`和`编辑`不同配置项分组和变量 ，快速完成后台配置变量设置。

支持通过权限控制，对 `敏感配置项` 信息进行 `安全隐藏` ，保障敏感数据安全。 



## 后台实时通知

通过弹窗和音频播放等方式 `实时通知` 后台管理员关键信息。

支持 `自定义` 消息类型通知音频；支持通过 `通知策略` 为不同管理员定制可接收的消息类型。

> 基于websocket 长连接，需要安装模块市场的 `workerman工程` ，具体配置请参考：[workerman工程模块](https://modules.buildadmin.com/workerman)
>
> 目前支持的通知类型：用户下单、取消订单、申请售后、商品库存预警、订单导出完成 



##  **在线客服** 

对接 `微信官方客服系统`，可在客服后台配置各种咨询信息。客户端一键跳转客服咨询界面，方便快捷。

客服后台请访问：[微信公众平台客服登录](https://mpkf.weixin.qq.com)



## 多种注册/登录方式

支持 `账号密码` 、`短信验证码` 、`微信手机号授权` 多种注册/登录方式，满足各种登录需求。

> 验证码功能需要安装模块市场的 `短信发送` ，具体配置参考：[短信发送模块](https://modules.buildadmin.com/sms)



## 自动登录&无感刷新

用户在 `微信小程序` 使用手机号授权登录后，后续进入登录页将 `自动完成登录` 操作，无需再手动登录。

登录令牌过期时系统会自动完成令牌置换续期后完成请求，此过程不会打断用户操作，提升用户体验。



## 商品分享

支持通过 `微信分享` 、`海报分享` 、`链接分享`  等方式分享商品，被分享者可通过链接和二维码快捷进入商品详情



# 演示地址

## 后台

体验后台请访问： [JoyShop商城后台](https://shop.joysplay.cn/#/admin) （为保障体验效果，已限制数据操作权限）

账号：`joyshop`

密码：`123456`



## 微信小程序

扫码体验或微信搜索  `JoyShop商城` 小程序

![](https://static-web.joysplay.cn/joyshop_qrcode.png)



## H5网页端

扫码体验

![](https://static-web.joysplay.cn/joyshop_h5.png)



# 项目展示

## 后台

![在这里插入图片描述](https://static-web.joysplay.cn/1.png)



![](https://static-web.joysplay.cn/2.png)



![](https://static-web.joysplay.cn/3.png)



![](https://static-web.joysplay.cn/4.png)



![](https://static-web.joysplay.cn/5.png)



![https://static-web.joysplay.cn/6.png](https://static-web.joysplay.cn/6.png)



![https://static-web.joysplay.cn/7.png](https://static-web.joysplay.cn/7.png)





## 移动端

<img src="https://static-web.joysplay.cn/mobile/1.png"  style="zoom: 15%; float:left" /> <img src="https://static-web.joysplay.cn/mobile/2.png" style="zoom: 15%; float:right" />































<img src="https://static-web.joysplay.cn/mobile/3.png" alt="https://static-web.joysplay.cn/mobile/3.png" style="zoom: 15%; float:left" /> <img src="https://static-web.joysplay.cn/mobile/4.png" style="zoom: 15%; float:right" />































<img src="https://static-web.joysplay.cn/mobile/5.png" style="zoom: 15%; float:left" /> <img src="https://static-web.joysplay.cn/mobile/6.png" style="zoom: 15%; float:right" />

 







 





















<img src="https://static-web.joysplay.cn/mobile/7.png" style="zoom: 15%; float:left" /> <img src="https://static-web.joysplay.cn/mobile/8.png" style="zoom: 15%; float:right" />

































<img src="https://static-web.joysplay.cn/mobile/9.png" style="zoom: 15%; float:left" /> <img src="https://static-web.joysplay.cn/mobile/10.png" style="zoom: 15%; float:right" /> 





































