<template>
  <div class="container">
    <!-- {{directs[0].name}} -->
    <ul class="d_icon">
        <li v-for="item in data" :key="item">
            <a :href="item.href">
                <img v-bind:src="`./images/directs/${item.src}`" alt="">
                <div class="txt">
                    {{item.name}}
                </div>         
            </a>
        </li>        
        <!-- <li v-for="item in directs" v-bind:key="item"> 
            <a :href="item.href">
                <img v-bind:src="`./images/directs/${item.src}`" alt="">
                <div class="txt">
                    {{item.name}}
                </div>         
            </a>
        </li> -->
    </ul>
  </div>
</template>

<script>
    // import directs from "../data/directs.js"(App.vue)
export default {
    props:["data"], //data를 받아준다.
    data(){
        return {
            // directs:directs(App.vue)
        }
    }
}
</script>

<style lang="scss">
    .d_icon{
        display: flex;
        gap:20px;
        li{
            _width: 10%;
        }
        img{
            width: 100%;
        }
        .txt{
            text-align: center;
        }
    }

</style>