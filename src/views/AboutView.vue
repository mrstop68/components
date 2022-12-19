<template>
  <div class="about">
    <h1>This is an about page</h1>
    <UserList @data="xDatax=$event" :userName='icerik'/>
    <button type="button" class="btn btn-primary" @click="degistir"> degistir</button>
    <p></p>
    <p>{{xDatax}}</p>
   
  </div>
</template>
<script>

import UserList from '@/components/UserList.vue'

export default {
  name: 'AboutView',
  components: {
    UserList,
},
  data() {
    return {
     xDatax: '',
     icerik:'bu metin about sayfasından userlist sayfasına gönderiliyor',
    }
  },
  methods: {
    degistir(){
     this.icerik='hebele hübele'
    }
  },
}
</script>
<style>

</style>
