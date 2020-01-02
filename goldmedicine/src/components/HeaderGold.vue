<template>
  <div class="headerGold">
    <div class="goldCenter headerFlex">
      <div class="navLinkLogin">欢迎进入金象网</div>
      <ul>
        <li class="nameList" v-for="(item,index) in headerName" :key="index" v-text="item.name"></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderGold",
  data: () => {
    return {
      headerName: [
        {
          name: "购物车"
        },
        {
          name: "我的订单"
        },
        {
          name: "个人中心"
        },
        {
          name: "关注金象网"
        },
        {
          name: "客户服务"
        }
      ]
    };
  }
};
</script>

<style scoped>
.headerGold {
  height: 30px;
  background: #f3f3f3;
  line-height: 30px;
}

.navLinkLogin {
  width: 190px;
  height: 100%;
}

.headerFlex {
  display: flex;
}

ul {
  flex: 1;
  margin: 0;
  padding: 0;
}
.nameList {
  float: left;
  line-height: 30px;
}
</style>
