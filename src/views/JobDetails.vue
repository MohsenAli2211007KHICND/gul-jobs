<template>
  <h1>Jobs detail</h1>
  <p>job's id is {{ id }}</p>
</template>

<script>
export default {
    data (){
        return {
            id: this.$route.params.id
        }
    }
}
</script>

<style>

</style>