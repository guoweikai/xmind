### 目录结构
pages.json : 配置页面路由,导航条,选项卡(工具栏)
mainfest


###  全局变量 globalData
在app.vue 中 
<script>
  export default {
    globalData:{
      msg:"hello world"
    }
  }
</script>

//在其他页面调用/修改全局变量

getApp().globalData.msg = "hello world"

注意:页面刷新数据就消失了

### vue ,小程序, uni-app 的生命周期

vue 四步

小程序 ui-app

onLoad: 首次进入页面加载时触发,可以在 onLoad 的参数中获取打开当前页面路径中的参数
onShow: 加载完成后,后台切到前台或重新进入页面时触发
onReady: 页面首次渲染完成时触发
onHide: 从前台切到后台或进入其他页面触发
onUnload: 页面卸载时触发
onPullDownRefresh: 监听用户下拉动作
onReachBottom: 页面上拉触低事件的处理函数
onShareAppMessage:用户点击右上角转发

