<template>
  <form>
    <!-- the default clicker -->
    <input class="butto" @click="count++" type="button" value="add to the count">

    <!-- The ultimate clicker once you achieve 69 -->
    <input class="butto" v-if="count >= 10" @click="count *= 2" type="button" value="double your add to the count">

    <input v-if="count >= 10" @click="count /= 10" type="button" class="butto" value="divide your count by 10">
  </form>
  <h1>the current count, is {{ count }}</h1>
  <p>Your goal, is to reach the coveted number, 69. because I have great humor</p>
</template>


<script>

  export default {
    data() {
      return {
        count: 0
      }
    }
  }

</script>