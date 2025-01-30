<script>
import { ref } from 'vue'

let date = new Date();
let year = date.getFullYear();
let month = date.getMonth() + 1;
let day = date.getDate();

export default {
  setup() {
    year: ref(year);
    month: ref(month);
    day:  ref(day);

    return {
      year,
      month,
      day,
    }
  },
  name: "Date",
}
</script>

<template>
  <h1>{{ year }}년 {{ month }}월 {{ day }}일</h1>
</template>

<style>
h1 {
  color: #152b4a
}
</style>
