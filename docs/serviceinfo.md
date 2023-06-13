
# 服务目录

| 服务名                                                | 服务描述                                                                                                                        |
| ----------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| [fy-erp-complaint-service](#fy-erp-complaint-service) | 投诉（含电商订单投诉）                                                                                                          |
| fy-erp-inventory-configure-service                    | 仓库标签设置；（其他仓库库存相关配置）                                                                                          |
| fy-erp-inventory-platform-service                     | 平台库存设置：  <br>平台可用库存类型、活动锁库存、同步比例等设置                                                                |
| fy-erp-o2o-service                                    | 全渠道服务                                                                                                                      |
| fy-erp-online-configure-service                       | 电商基础配置：  <br>电商相关的基础码表；  <br>平台、网店维护；  <br>承运商维护；  <br>订单相关策略配置；                        |
| fy-erp-online-order-evaluate-service                  | 线上订单评价查询、回复  <br>-aimer：为爱慕客户化服务包                                                                          |
| fy-erp-online-order-service                           | 电商订单相关服务（线上订单相关的查询、处理、订单查询报表）                                                                      |
| fy-erp-online-work-order-service                      | 工单服务                                                                                                                        |
| fy-middleware-service                                 | 中间件服务（多服务模块协同）                                                                                                    |
| fy-promotion-online-service                           | 电商可参与促销、包材服务                                                                                                        |
| fy-promotion-online-service                           | 电商订单判断满足的促销服务（仅适用于促销中心版本）                                                                              |
| fy-tp-aftersale-service                               | 平台订单售后申请查询、同意  <br>-aimer：为爱慕客户化服务包                                                                      |
| fy-tp-aftersale-treatment-job                         | 平台售后处理：发货前自动退款，自动生成退货单等  <br>-aimer：为爱慕客户化服务包                                                  |
| fy-tp-client-[平台]                                   | 6.1订单抓单（时间片、推单模式）                                                                                                 |
| fy-tp-dispatch                                        | 订单绑定赠品、快递分配、寻仓                                                                                                    |
| fy-tp-item-download-job                               | 平台商品的定时下载任务                                                                                                          |
| fy-tp-item-service                                    | 平台商品的查询、手工下载、重新上传库存等服务                                                                                    |
| fy-tp-item-upload-inventory-job                       | 库存同步                                                                                                                        |
| fy-tp-order-decode-service                            | 脱敏订单解密服务                                                                                                                |
| fy-tp-order-local-job                                 | 6.1订单保存（tp_order_*** 至：ECT010）                                                                                          |
| fy-tp-order-upload-state-job / task                   | 订单状态回传（-job：无kafka版   -task：kafka版）  <br>支持原单、拆单发货出库；退货入库、换发出库；                              |
| fy-tp-promotion-standard                              | 电商订单促销绑定赠品（调用：fy-promotion-online-service）                                                                       |
| fy-tp-self-modify-service                             | 平台订单自助修改地址、改商品                                                                                                    |
| fy-tp-self-modify-service-cloud                       | 平台订单自助修改商家路由跳转云服务  <br>针对一个Appkey只能配置一个SPI路由是，使用此服务地址，跳转分发到实际商家自助改地址服务   |
| fy-tp-self-modify-service-forward                     | 平台自助修改消息广播JOB  <br>用于平台无法将订单自助修改信息通过SPI通知ISV时，采用此服务模拟平台通过SPI调用ISV的自助改地址服务； |
| fy-tp-stock-alloc-aimer                               | 【Aimer】ECT020.ECZYBZ=1的商品确定库存分布                                                                                      |
| fy-tp-tune-warehouse                                  | 指定仓库处理任务                                                                                                                |
| fy-wms-express-order-service                          | 平台获取运单与电子面单内容服务                                                                                                  |
| [fy-tp-order-local-job](#fy-tp-order-local-job)                            | 订单保存任务与其它相关查询服务                                                                                                  |


# 服务说明

## fy-erp-complaint-service

投诉（含电商订单投诉）1


## fy-tp-order-local-job

- 订单保存定时任务服务
- 手工抓单服务
- 订单待保存队列查询
- 订单售后申请解析与保存队列查询
- 订单换货申请解析与保存队列查询
- 平台订单流转情况查询
- 平台订单解析结果查询
