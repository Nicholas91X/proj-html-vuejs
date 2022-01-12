<template>
  <div id="card-services">
      <div class="image">
        <img :src="info.img" :alt="info.title">
        <div class="right-arrow">
            <i class="fas fa-arrow-right"></i>
        </div>
      </div>
      <div class="title">
          <h4>{{info.title}}</h4>
      </div>
      <div class="text">
          <p>{{info.text}}</p>
      </div>
  </div>
</template>

<script>
export default {
    name: "CardServices",
    props: {
        info: Object
    }
}
</script>

<style lang="scss" scoped>
@import '../../assets/variables.scss';
    #card-services {
        width: calc(100% / 3 - 60px);
        margin: 10px;
        background-color: white;
        border-radius: 5px;
        text-align: left;
        padding: 20px;
        .image {
            display: flex;
            justify-content: space-between;
            .right-arrow {
                color: $elm; 
                font-size: 15px;  
            }
        }
        .title {
            font-size: 15px;
        }
        .text {
            color: $pumice;
        }
    }
</style>