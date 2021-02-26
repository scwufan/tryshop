<template>
 <div>
 
 </div>
</template>

<script>
import axios from 'axios'
 export default {
   name: '',
   props: {
   },
   components: {

   },
   data () {
     return {
       data:[],

     }
   },
   methods: {

   },
   mounted() {
     axios.get('http://192.168.101.98:7001/shoplist/getShop').then((res) =>{
        console.log(res)
        this.data= res
     })
   },
   watch: {

   },
   computed: {

   }
 }
</script>

<style scoped lang='scss'>

</style>