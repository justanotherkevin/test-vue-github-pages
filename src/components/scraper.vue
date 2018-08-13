<template>
  <div class="scraper-wrapper" id='scraper'>
    <input type="text" name="" id="" placeholder='drop URL here' v-model='url'>
    <button type="submit" v-on:click='submitSearchUrl'>Scrape</button>
  </div>
</template>

<script>
export default {
  name: 'scraper',
  data () {
    return {
      url: '',
      submitCooldown: null
    }
  },
  methods: {
    submitSearchUrl: () => {
      if (this.submitCooldown) {
        alert('you doing it too offten')
      } else {
        this.submitCooldown = true
        setTimeout(() => {
          this.submitCooldown = null
        }, 3000)
      }
    }
  }
}
</script>
