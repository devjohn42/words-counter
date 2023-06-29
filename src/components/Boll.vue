<template>
  <div class="boll">
    <span class="word">{{ word }}</span>
    <span class="amount">{{ amount }}</span>
  </div>
</template>

<script>
export default {
  props: ["word", "amount"],
};
</script>

<style scoped>
.boll {
  background-color: green;
  height: 55px;
  width: fit-content;

  margin: 10px;
  padding: 1rem;
  border-radius: 35px;

  font-weight: bold;

  display: flex;
  gap: 10px;
  align-items: center;
  justify-content: center;
}

.boll .word {
  color: #ffffff;
  font-size: 1.3rem;
}

.boll .amount {
  background-color: #ffffff;
  width: 40px;
  height: 40px;
  border-radius: 50%;

  /* padding: 5px; */

  font-size: 0.9rem;
  color: green;
  
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
