<template>
  <div class="topNav">
    <div class="topleft">
      <svg class="icon" aria-hidden="true">
        <use xlink:href="#icon-31liebiao"></use>
      </svg>
    </div>

    <div class="topContent">
      <span @click="$router.push('/Login')">我的</span>
      <span class="active">首页</span>
      <span>榜单</span>
    </div>
    <div class="topRight">
      <svg class="icon" aria-hidden="true" @click="$router.push('/search')">
        <use xlink:href="#icon-sousuo"></use>
      </svg>
    </div>
  </div>
  
</template>
<style lang="less" scoped>
    .topNav{
        width: 100%;
        height: 1rem;
        padding: .2rem;
        display: flex;
        justify-content: space-between;
        align-items: center;
        .topContent{
            width: 65%;
            height: 100%;
            display: flex;
            justify-content: space-around;
            // align-items: center;
            font-size: .36rem;
            .active{
                font-weight: 900;
            }
        }
    }
</style>