<template>
  <div class="bolls">
    <Boll
      v-for="item in groupedWords"
      :word="item.word"
      :amount="item.amount"
      :key="item.word"
    />
  </div>
</template>

<script>
import Boll from "./Boll.vue";
export default {
  components: {
    Boll,
  },
  data: function () {
    return {
      groupedWords: [
        { word: "i", amount: 547 },
        { word: "you", amount: 478 },
        { word: "it", amount: 10 },
      ],
    };
  },
};
</script>

<style scoped>
.bolls {
  display: flex;
}
</style>
