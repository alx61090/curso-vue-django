<template>
  <h1>Listado</h1>
</template>


<script>
export default{
  mounted(){
    this.$axios.get('http://127.0.0.1:8000/api/category/all/?format=json').then((res)=>{
      console.log(res.data)
    })
  }
}
</script>