<template>
    <div class="container">
        <header class="header">
            <div class="home-text">
                <p>Github</p>
                <span>Search</span>
            </div>
            <FormStyled/>
        </header>
        <aside class="aside">
            <div class="aside-user">
                <img src="" alt="" width="300" height="300">
                <h2>Edson Bastos</h2>
                <h3>edsonbastos2</h3>
            </div>
            <div class="aside-organization">
                <ul>
                    <li>
                        <img src="@/assets/icon1.png" alt="">
                        <span>Empresa</span>
                    </li>
                    <li>
                        <img src="@/assets/icon2.png" alt="">
                        <span>cidade</span>
                    </li>
                    <li>
                        <img src="@/assets/icon3.png" alt="">
                        <span>0</span>
                    </li>
                    <li>
                        <img src="@/assets/icon4.png" alt="">
                        <span>4</span>
                    </li>
                    <li>
                        <img src="@/assets/icon6.png" alt="">
                        <span>1</span>
                    </li>
                </ul>
            </div>
        </aside>
        <main class="main">
            <div class="content">
                <div class="content-main">
                    <h1>Titulo</h1>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                        Unde, est saepe assumenda vel voluptates nemo nobis ut molestias? 
                        Temporibus labore ipsam minima pariatur praesentium assumenda ipsum obcaecati soluta, 
                        doloribus eligendi.
                    </p>
                    <div class="follow">
                        <img src="@/assets/icon4.png" alt=""><span>0</span>
                    </div>
                </div>
                <div class="content-main">
                    <h1>Titulo</h1>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                        Unde, est saepe assumenda vel voluptates nemo nobis ut molestias? 
                        Temporibus labore ipsam minima pariatur praesentium assumenda ipsum obcaecati soluta, 
                        doloribus eligendi.
                    </p>
                    <div class="follow">
                        <img src="@/assets/icon4.png" alt=""><span>0</span>
                    </div>
                </div>
                <div class="content-main">
                    <h1>Titulo</h1>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                        Unde, est saepe assumenda vel voluptates nemo nobis ut molestias? 
                        Temporibus labore ipsam minima pariatur praesentium assumenda ipsum obcaecati soluta, 
                        doloribus eligendi.
                    </p>
                    <div class="follow">
                        <img src="@/assets/icon4.png" alt=""><span>0</span>
                    </div>
                </div>
            </div>
        </main>
    </div>
</template>

<script>
import FormStyled from '@/components/FormStyled.vue'
    export default {
        components:{
            FormStyled
        }
    }
</script>

<style scoped>
.container{
    display: grid;
    grid-template-columns: 300px 1fr;
    grid-template-rows: 50px 1fr;
    grid-template-areas: 
    'header header'
    'aside main';
    grid-gap: 1rem;
}
.header{
    grid-area: header;
}
.aside{
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    grid-area: aside;
    font-family: 'Rubik', sans-serif;
}

.aside-user{
    display: flex;
    flex-direction: column;
}

.aside-user h2{
    font-style: normal;
    font-weight: 300;
    font-size: 36px;
    color: #000;
    line-height: 43px;
    margin-bottom: -20px;
}

.aside-user h3{
    font-style: normal;
    font-weight: 300;
    font-size: 24px;
    line-height: 28px;
    color: #757575;
}
.aside-organization ul{
    padding: 0px;
    display: flex;
    flex-direction: column;
    align-content: center;
    align-items:flex-start ;
}
.aside-organization li{
    list-style: none;
    display: flex;
    justify-content: center;
    align-items: baseline;
    margin-bottom: 20px;
}
.aside-organization ul li span{
    margin-left: 10px;
}

.main{
    grid-area: main;
    font-family: 'Rubik', sans-serif;
}

.content-main h1{
    font-weight: 300;
    font-size: 36px;
    line-height: 43px;
}

.content-main p{
    font-weight: 300;
    font-size: 24px;
    line-height: 28px;
    color: #757575;
}
.follow{
    display: flex;
    align-items: baseline;
}
.follow span{
    font-size: 20px;
    color: #757575;
}
.header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    align-content: center;
}
.home-text{
    margin-bottom: 0;
}
.home-text p, .home-text span{
    font-size: 42px;
}
</style>