<template>
    <div>
        <p >{{userName}}</p>
        <button @click="goster">Parent e gönder</button>
    </div>
</template>
<script>
export default {
    name: 'UserList',
    props:['userName'],
    data(){
        this.$emit('data', 'tıklamadan hebele hübele')
        return{
           
        }
    },
methods:{
    goster(){
        this.$emit('data', 'tıkladıktan sonra hopppala')
    }
}  
}
</script>