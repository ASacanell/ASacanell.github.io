<template>
  <div>
    <div class="h-4 bg-primary w-full" />
    <div class="pt-10 pb-10 flex justify-center">
      <div class="w-1/2">
        <intro />
        <extract class="mt-10" />
      </div>
    </div>
  </div>
</template>

<script>
  import Intro from '~/components/Intro.vue'
  import Extract from '~/components/Extract.vue'

  export default {
    components: {Intro, Extract},

    data () {
      return {
        online: true
      }
    },

    mounted () {
      if (!window.navigator) {
        this.online = false
        return
      }
      this.online = Boolean(window.navigator.onLine)
      window.addEventListener('offline', this._toggleNetworkStatus)
      window.addEventListener('online', this._toggleNetworkStatus)
    },

    methods: {
      _toggleNetworkStatus ({ type }) {
        this.online = type === 'online'
      }
    },

    destroyed () {
      window.removeEventListener('offline', this._toggleNetworkStatus)
      window.removeEventListener('online', this._toggleNetworkStatus)
    }
  }
</script>