# Notes
This  is repository to  recoding ntoes

test 1111

ctrl shift  t  提交

commint

//下单json
{"pcorder":{"total_number":200,"totall_price":300,"buyerId":"购买方id"},"pcorderNo":"批次号","orders":[{"total_number":100,"totall_price":150,"seller_ID":"卖方id","companyID":"购买方id","invoiceTYPE":"发票类型","invoiceHead":"发票抬头","invoiceContent":"发票内容","invoiceHeadType":"发票抬头类型","provinceName":"省","cityName":"市","areaName":"区","address":"地址","postNumber":"邮编","consigneeName":"收货人姓名","mobile":"收货人手机","telephone":"电话","remark":"备注 .payType 0现金 1 挂账","payType":0,"logisticsCode":"55d7251de5ef4aa78667e32abcfeec67","logisticsCompany":"小猪物流",
"detils":
[{"goods_id":"商品表内编号id","goods_amount":100,"goods_price":150,"goods_name":"商品名称","factoryId":"商品厂家编码factoryId"}]}
]

}

//收货 json
0 订单部分收货 1  订单已完成确认收货
{"state":1,"indentId":"DD20170912151941595000","logisticsId":"fh20170912154033228001","receiveGood":{"receivetotal":100},
"detils":
[{"goodId":"商品表内编号 Id","goodNumber":100,"goodName":"商品名称"}]
}
//买家取消订单
{"listIndent":
["DD20170912162253177000"]
}
//买家申请退货

{
"indentId":"DD20170912162253177000","buyId":"买家id","returnOrder":{"returnNumber":20,"remarks":"退货备注"},
"returnDetails":
[{"returnNumber":20,"goodId":"商品id"}]

}




代表订单状态
12101001	1210	待提交
12101002	1210	已提交
12101003	1210	已取消
12101004	1210	已驳回
12101005	1210	待接单    0.待接单
12101006	1210	待发货 1.已接单  2财务已审核
12101007	1210	待收货    3.已发货,待收货   4买家确认部分收货
12101008	1210	已完成     5 买家全部收货

代表退货单状态
12101009	1210	退货申请 0  待审核
12101010	1210	退货中    1  销售审核   2 仓库审核
12101011	1210	拒绝退货  11  拒绝退货
12101012	1210	已退货     3 财务审核
