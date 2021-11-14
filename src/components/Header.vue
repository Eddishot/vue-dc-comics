<template>
    <div class="header-container">
         <img src="../assets/dc-logo.png" alt="Dc Logo" />

         <ul>
             <li v-for="item, i in navbarItems" :key="i">{{item.title}}</li>
         </ul>

    </div>


</template>


<script>

export default {

    name:"Header",

    data(){

        return{

            navbarItems:[
                {
                    title:"CHARACTERS",
                    href:"#"
                },
                {
                    title:"COMICS",
                    href:"#"
                },
                {
                    title:"MOVIES",
                    href:"#"
                },
                {
                    title:"TV",
                    href:"#"
                },
                {
                    title:"GAMES",
                    href:"#"
                },
                {
                    title:"COLLECTIBLES",
                    href:"#"
                },
                {
                    title:"VIDEO",
                    href:"#"
                },
                {
                    title:"FANS",
                    href:"#"
                },
                {
                    title:"NEWS",
                    href:"#"
                },
                {
                    title:"SHOP",
                    href:"#"
                },
            ]
        }
    }
}

</script>



<style lang="scss" scoped>

    .header-container{
        display:flex;
        align-items:center;
        justify-content:space-between;
        margin:auto;
        padding-top:15px;
        width:1200px;
    }

    ul {

        list-style:none;

        li{
            display:inline-block;
            font-size:17px;
            font-weight:bold;
            padding: 0 6px;
        }
    }


</style>