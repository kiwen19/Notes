# Notes
This  is repository to  recoding ntoes

test 1111

ctrl shift  t  提交

commint

//下单json
{"pcorder":
{"total_number":200,"totall_price":300,"buyerId":"购买方id"},
"pcorderNo":"批次号",
"orders":
[{"total_number":100,"totall_price":150,"seller_ID":"卖方id","companyID":"购买方id","invoiceTYPE":"发票类型","invoiceHead":"发票抬头","invoiceContent":"发票内容","invoiceHeadType":"发票抬头类型","provinceName":"省","cityName":"市","areaName":"区","address":"地址","postNumber":"邮编","consigneeName":"收货人姓名","mobile":"收货人手机","telephone":"电话","remark":"备注/s payType 0现金 1 挂账","payType":0,
"detils":[{"goods_id":"商品表内编号id","goods_amount":100,"goods_price":150,"goods_name":"商品名称","factoryId":"商品厂家编码factoryId"}]
}]

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
