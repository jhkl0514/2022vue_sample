<template>
  <div class="container">
    <!-- {{directs[0].name}} -->
    <ul>
        <li v-for="item in directs" v-bind:key="item">
            <!-- {{item}} -->
            <img v-bind:src="`./images/directs/${item.src}`" alt="">           
        </li>
    </ul>
  </div>
</template>

<script>
    import directs from "../data/directs.js"
export default {
    data(){
        return {
            directs:directs
        }
    }
}
</script>

<style>

</style>