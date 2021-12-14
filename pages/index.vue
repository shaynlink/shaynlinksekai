<template>
  <div class="sekai_container">
    <div class="sekai_hello">
      <div>
        <img src="~/static/me-memoji-hello.webp" />
      </div>
      <div>
        <h1>Hey everyone !</h1>
        <h3>I'm rayane</h3>
        <h3>{{age}} year old french student developer</h3>
      </div>
    </div>

    <div>
      
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  data() {
    const now = Date.now();
    const myAge = Date.parse(new Date(2003, 6, 29).toString());

    return {
      age: new Date(now - myAge).getFullYear() - 1970
    }
  }
})
</script>

<style lang="scss" scoped>
.sekai_hello {
  display: flex;
  justify-content: center;
  align-items: center;
  height: calc(100vh - 86px);
  width: 100%;
}
</style>