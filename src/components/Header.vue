<template>
    <div class="header-container">
         <img src="../assets/dc-logo.png" alt="Dc Logo" />

         <ul>
                <li v-for="item, i in navbarItems" :key="i">
                    <a :href="item.href">{{item.title}}</a>
                </li>
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
        padding:15px 0;
        width:1200px;

        img{
            width: 60px;
            // padding-bottom: 10px;
        }
    }

    ul {

        list-style:none;

        li{
            display:inline-block;
            font-size:17px;
           
            padding: 0 6px;

            a{
                text-decoration: none;
                color: black;
                font-weight:bold;

                &:hover{
                    color: #2196f3;
                    border-bottom: 2px solid #2196f3 ;
                }
            }
        }
    }


</style>