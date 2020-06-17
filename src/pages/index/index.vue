<template>
  <div class="index-body">
    <div class="book-card">
      <span style="font-size: 12px">目的地</span>
      <div class="location-body">
        <section class='set-location-style'>深圳</section>
        <section class='my-location-tips-style'>我的位置</section>
      </div>
    </div>
  </div>
</template>

<script>
import SearchBar from "@/components/search/SearchBar";

export default {
  data() {
    return {
      hotSearch: {
        keyword: "搜索"
      }
    };
  },

  components: {
    SearchBar
  },

  methods: {
    onSearchBarClick() {}
  },

  created() {
    // let app = getApp()
  }
};
</script>

<style lang='scss' scoped>
.index-body {
  position: relative;
  border-top: 1px solid #e7e7e7;

  .book-card {
    height: 220px;
    position: absolute;
    top: 110px;
    left: 16px;
    right: 16px;
    background-color: red;
    border: 1px solid #e7e7e7;
    border-radius: 4px;
    padding: 16px;
    box-sizing: border-box;
  }

  .location-body {
    display: flex;
    justify-content: space-between;
  }
}
</style>
