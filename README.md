# sparkdesk
## 简介
我的毕设进行中，无意发现这个bug...
毕设vue3，但该组件基于vue2，可在vue3中直接使用

## 功能
大模型返回消息后不会主动保留消息记录，消息历史又开发者主动调用
在调用前用于通过界面自定义消息记录，实现篡改消息记录
一定程度上可以实现诱导大模型回答敏感问题，但不建议

## 使用
找到data函数，填写应用id、应用密钥等，应用可在[讯飞开发平台](https://console.xfyun.cn/app/myapp)申请
`export default {
  data() {
    return {
      appId: "",     //填写appId
      apiKey: "",    //填写apiKey
      apiSecret: "", //填写apiSecret
      ...
`
填写完成后即可生效，放在任意一个vue项目中使用，可直接提问

![界面](./sparkdesk.png "界面")