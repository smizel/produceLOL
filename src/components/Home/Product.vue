<template>
  <div class="page">
    <Header :game="game" :pro="pro"></Header>


    <div class="content">
      <div class="msg_hot">
        <div class="msg_left">
          <img src="../../assets/img/top.png" alt="">
          <p>周边信息</p>
          <span class="msg_left_time">
            2018-9-18
          </span>
          <span class="msg_left_num">
            1.7万阅读量
          </span>
        </div>
        <div class="msg_right">
          <img src="../../assets/img/a.png" alt="">
        </div>
      </div>
    </div>


    <Footer :home_gol="gol" :discuss_gol="discuss_gol" :match_gol="match_gol" :data_gol="data_gol"></Footer>

  </div>
</template>

<script>
  export default {
    name: "Product",
    data () {
      return {
        product:'周边',
        pro:'active',
        discuss_gol : require('../../assets/img/discuss.png'),
        gol : require('../../assets/img/home1.png'),
        match_gol : require('../../assets/img/match.png'),
        data_gol : require('../../assets/img/data.png'),
        game : require('../../assets/img/lol.png'),
      }
    }
  }
</script>

<style scoped>
  @import "../../assets/css/information.css";
  .content {
    margin-top: 90px;
  }
</style>
