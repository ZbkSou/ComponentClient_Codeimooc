# 组件化思维变成android

## 首页开发

开发tab多fragment类型首页 ，首页一般启动模式设置成单例
操作fragment 的时候 detach 和attach 不会销毁fragment 但是会销毁其中的view 
replace 会移除栈中的所有fragment 

## 网络封装思想

### 封装request 

RequestParams  保存请求参数
ConcurrentHashMap 线程安全的map
CommonRequest 用来返回request

### 封装发送请求，参数 https

CommonOkHttpClient 封装对外网络请求方法
设置超时时间
### 封装callback 
异常 解析 线程转发

DisposeDataListener 会毁掉监听
