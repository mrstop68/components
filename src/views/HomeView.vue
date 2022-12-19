<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <hello-world :msg="title"></hello-world>
    <hr>
    <UserHome/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import UserHome from '@/components/UserHome.vue'
export default {
  name: 'HomeView',
  components: {
    HelloWorld,
    UserHome
  },
  data() {
    return {
      title: 'hoppele'
    }
  },
}
</script>
