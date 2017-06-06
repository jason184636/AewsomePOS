<template>
    <div class="pos">
      <el-row>
        <el-col :span="7" class="pos-order" id="order-list">
          我是订单栏
        </el-col>
        <el-col>
          我是产品栏
        </el-col>
      </el-row>
    </div>
</template>

<script type="text/ecmascript-6">
    export default{
        name: 'pos',
        mounted: function(){
            var orderheight=document.body.clientHeight;
            console.log(orderheight);
            document.getElementById('order-list').style.height=orderheight+'px';
        }
        //mounted 钩子函数，在虚拟dom 加载之后，这里实行
    }
</script>

<style lang="" rel="stylesheet/text">
  .pos-order{
    background-color: #f9fafc;
    border-right: 1px solid #c0ccda;
  }
</style>
