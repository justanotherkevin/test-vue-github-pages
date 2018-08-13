<template>
  <div class='test'>
    <h1 v-text='title'></h1>
    <button v-if='!changeTitle' v-on:click='toggleChangeTitleState'>Change title</button>
    <div    v-else>
      <input type='text' v-model='title' >
      <button v-on:click='toggleChangeTitleState'>Close</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'test',
  data () {
    return {
      title: 'hello vue',
      changeTitle: false
    }
  },
  methods: {
    toggleChangeTitleState: function () {
      this.changeTitle = !this.changeTitle
    }
  }
  // computed: {

  // }
}
</script>

<style scoped >
</style>
