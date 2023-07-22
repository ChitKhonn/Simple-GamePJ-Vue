<template>
  <div>
    <p>Result is {{ score }} ms </p>
    <div v-if="score < 250">
      Wow... You are click skill is too fast!
    </div>
    <div v-else-if="score > 250 && score < 500">
      You are click skill is normal!
    </div>
    <div v-else>
      You are click skill is slow, try again!
    </div>


  </div>
</template>

<script>
export default {
    props:['score']
}
</script>

<style>

</style>