<template>
  <img :style="{ height: imgHeight, 'vertical-align': verticalAlign }" />
</template>

<script>
export default {
  props: ['height'],
  data () {
    return {
      verticalAlign: 'text-bottom'
    }
  },
  computed: {
    imgHeight () {
      return this.height ? this.height : '1.5em'
    }
  }
}
</script>
