<template>
  <div class="home">
    <div class="home-text">
      <p>Github</p>
      <span>Search</span>
    </div>
   <Form/>
  </div>
</template>

<script>
// @ is an alias to /src
import Form from "@/components/FormStyled.vue"
export default {
  components:{
    Form,
  },
  name: "Home",
};
</script>

<style scoped>
.home{
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

</style>
