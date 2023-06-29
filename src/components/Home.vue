<template>
  <div class="home">
    <v-form>
      <v-file-input
        label="Selecione as legendas"
        prepend-icon="mdi-message-text"
        append-icon="mdi-send"
        outlined
        multiple
        v-model="files"
        @click:append="filterSubtitles"
      >
      </v-file-input>
    </v-form>
    <div class="bolls">
      <Boll
        v-for="item in groupedWords"
        :word="item.word"
        :amount="item.amount"
        :key="item.word"
      />
    </div>
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
      files: [],
      groupedWords: [
        { word: "i", amount: 547 },
        { word: "you", amount: 478 },
        { word: "it", amount: 10 },
      ],
    };
  },
  methods: {
    filterSubtitles() {
      console.log(this.files);
    },
  },
};
</script>

<style scoped>
.home {
  margin: 20px;
}
.bolls {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
</style>
