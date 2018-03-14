<template>
  <div class="post">
      <el-row>
        <el-col :span='7' class="post-order" id="order-list">
          我是订单栏
        </el-col>
        <el-col :span='7'>
          我是产品栏
        </el-col>
      </el-row>
  </div>
</template>

<script>
export default {
  name:'pos',
  mounted:function(){
    var orderHeight=document.body.clientHeight;
    console.log(orderHeight);
    document.getElementById('order-list').style.height=orderHeight+'px';
  }
}
</script>

<style scoped>
.post-order {
  background-color: #f9fafc;
  border-right: 1px solid #c0ccda;
}
</style>
