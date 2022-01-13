<template>
  <div class="card-project">
      <img src="../../assets/img/project-1.jpg">
      <div class="title">{{info.title}}</div>
      <div class="text">{{info.text}}</div>
      <div class="layover"></div>
  </div>
</template>

<script>
export default {
    name: "CardProject",
    props: {
        info: Object
    }
}
</script>

<style lang="scss" scoped>
@import '../../assets/variables.scss';

.card-project {
    width: calc(100% / 3 - 20px);
    margin: 10px;
    height: 150px;
    border-radius: 5px;
    position: relative;
    overflow: hidden;
    .layover {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-color: rgba(0, 0, 0, .4);
    }
    .title,
    .text {
        position: absolute;
        text-align: center;
        color: white;
        z-index: 9999;
    }
    .title {
        bottom: 20px;
        font-weight: 700;
        font-size: 15px;
        padding: 0 10px;
    }
    .text {
    }
    img {
        width: 100%;
    }
}
</style>