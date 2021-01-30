<template>
  <div>
    <v-header></v-header>
    <main class="content-container" ref="container" :class="headFixed == true ? 'marginTop' : ''">
      <nuxt/>
    </main>
    <v-footer></v-footer>
  </div>
</template>
<script>
import VHeader from '~/components/home/header'
import VFooter from '~/components/home/footer'

export default {
   components:{
     VHeader,
     VFooter
   }
}
</script>
<style>
  .marginTop{
    margin-top: 170px;
  }
</style>
