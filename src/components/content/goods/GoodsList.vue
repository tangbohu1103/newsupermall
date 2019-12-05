<template>
    <div class="goods">
      <goods-list-item v-for="(item,itemIndex) in goods" :key="itemIndex" :goods-item="item"/>
    </div>
</template>

<script>
  import GoodsListItem from "./GoodsListItem"
    export default {
      name: "GoodsList",

      components:{
        GoodsListItem
      },

      props:{
          goods:{
            type:Array,
            default() {
              return [];
            }
          }
      }
    }
</script>

<style scoped>

</style>
