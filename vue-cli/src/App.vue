<template>
  <div>
    <AppHeader v-bind:propsdata="str" v-on:renew="renewstr" />
  </div>
</template>

<script>
  import AppHeader from './components/AppHeader.vue';

  export default {
    data: function(){
      return {
        str: 'Header'
      }
    },
    components: {
      AppHeader
    },
    methods: {
      renewstr: function(){
        this.str = 'hi';
      }
    }
  }
</script>

<style>

</style>