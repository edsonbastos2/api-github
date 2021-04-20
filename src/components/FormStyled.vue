<template>
    <form class="form-styled" action="">
        <input type="text" name="">
        <button>
            <img src="@/assets/search.png" alt="">
        </button>
    </form>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
.form-styled{
    display: flex;
}
.form-styled input{
    width: 600px;
    border: 2px solid #000;
    font-size: 20px;
    outline: none;
}
.form-styled button{
    width: 100px;
    height: 50px;
    background-color: #000;
    border-color: #000;
    outline: none;
}
</style>