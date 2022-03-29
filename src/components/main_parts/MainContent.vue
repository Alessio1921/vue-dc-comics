<template>
  <div class="card">
    <img :src="cardElement.thumb" alt="" srcset="">
    <p>{{cardElement.series}}</p>
  </div>
</template>

<script>
export default {
  name:"MainContent",
  props:['cardElement']

}
</script>

<style lang="scss" scoped>
  .card{
    width: 160px;
    height:160px;
    display: flex;
    flex-direction: column;
    padding: 1rem;
    img{
      height:100%;
      object-fit: cover;
      object-position: top;
    }
    p{
      font-size: .7rem;
    }
  }
</style>