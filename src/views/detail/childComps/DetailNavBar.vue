<template>
  <div>
    <nav-bar>
      <div slot="left" class="back" @click="backClick">
        <img src="~assets/img/common/back.svg" alt="">
      </div>
      <div slot="center" id="title">
        <div :key="(item,index)"
         v-for="(item,index) in titles"
         class="title-item"
         :class="{active:index===currentIndex}" @click="titleClick(index)">{{item}}</div>
      </div>
   </nav-bar>
  </div>
</template>

<script>
import NavBar from 'components/common/navbar/NavBar'

export default {
  components:{
    NavBar
  },
  data() {
    return {
      titles:['商品','参数','评论','推荐'],
      currentIndex:0,
    }
  },
  methods: {
    titleClick(index) {
      this.currentIndex=index
    },
    backClick() {
      this.$router.back()
    }
  },
}
</script>

<style scuped>
#title {
  display: flex;
}
.title-item {
  flex: 1;
}
.active {
  color: var(--color-high-text);
}
.back img {
  margin-top: 12px;
}
</style>
