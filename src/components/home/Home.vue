<template>
    <div>
        我是首页
        <mt-button type="danger" size="large">123</mt-button>
    </div>
</template>
<script type="text/ecmascript-6">
 export default {
     data(){
         return {

         }
     },created(){
         this.$ajax.get('getlunbo')
         .then(res=>{
             console.log(res);
         })
         .catch(err=>{
             console.log(err);
         })
     }
 }
</script>