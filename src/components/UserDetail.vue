<template>
    <div>
        <h4> {{metin}}</h4>
        <h6> {{ex}}</h6>
        <input type="text" name="" id="" v-model='tt'>
        <p >{{tt}}</p>
        <p >{{gelen}}</p>
    </div>
</template>
<script>
export default{
    name: 'UserDetail',
    props:['metin','ex'],
    
    data(){
        return{
            tt:'kk',
            gelen:this.ex
        }
    }
}

</script>
<style>

</style>