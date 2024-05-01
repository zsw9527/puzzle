<template>

  <div class="panel">
    <div @click="click(0, 0)"><img :src="imgs[0][0]"></div>
    <div @click="click(0, 1)"><img :src="imgs[0][1]"></div>
    <div @click="click(0, 2)"><img :src="imgs[0][2]"></div>
    <div @click="click(1, 0)"><img :src="imgs[1][0]"></div>
    <div @click="click(1, 1)"><img :src="imgs[1][1]"></div>
    <div @click="click(1, 2)"><img :src="imgs[1][2]"></div>
    <div @click="click(2, 0)"><img :src="imgs[2][0]"></div>
    <div @click="click(2, 1)"><img :src="imgs[2][1]"></div>
    <div @click="click(2, 2)"><img :src="imgs[2][2]"></div>
  </div>

</template>

<script>
export default {
  name: "GamePanel",
  props: {
    msg: String
  },
  data() {
    return {
      imgs: [
        ['/yjt/1714566185430_1.jpeg', '/yjt/1714566185430_2.jpeg', '/yjt/1714566185430_3.jpeg'],
        ['/yjt/1714566185430_4.jpeg', '/yjt/1714566185430_5.jpeg', '/yjt/1714566185430_6.jpeg'],
        ['/yjt/1714566185430_7.jpeg', '/yjt/1714566185430_8.jpeg', '/yjt/1714566185430_9.jpeg']
      ],

      click: function (x, y) {
        console.log('点击区域' + x + ',' + y)
        console.log(this.imgs[x, y])
      }
    }
  }

}
</script>

<style scoped>
.panel {
  margin-left: 33%;
  width: 600px;
  display: flex;
  flex-wrap: wrap;
}

.panel div {
  border: 1px solid black; /* 1px宽度，实线，黑色边框 */
  width: 33%;
  text-align: center;
  height: 200px;
}

.panel div img {
  width: 200px;
}

</style>