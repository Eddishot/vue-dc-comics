<template>
<section>
    <div class="background-primary">
        <div class="card-item-link">
            <div v-for="item, i in primaryLinks" :key="i" class="single-card">
               <div class="img-single-card">
                   <img :src="item.img" :alt="item.title">
                </div> 
                <h4>{{item.title}}</h4>
                
            </div>
        </div>
    </div>

    <div class="background-footer">
        <div class="container-DC-links">
            <div class="container-all-links">
                <div class="single-link">
                    <h5>DC COMICS</h5>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>Tv</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <h5>
                        SHOP
                    </h5>
                    <ul>
                        <li>Shop Dc</li>
                      

                        <li> Shop Dc Collectibles</li>
                    </ul>
                </div>
                <div class="single-link">
                    <h5>
                        DC
                    </h5>
                    <ul>
                        <li>Terms Of Use</li>
                        <li>Privacy policy(New)</li>
                        <li>Ad Choices</li>
                        <li>Ad Choices</li>
                        <li>Adversting</li>
                        <li>Job</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                </div>
                <div class="single-link">
                    <h5>SITES</h5>
                    <ul>
                        <li>Dc</li>
                        <li>MAD Magazine</li>
                        <li>Dc Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power VIsa</li>
                    </ul>

                </div>

            </div>

            <img src="../assets/dc-logo-bg.png" alt="LOGO DC">

        </div>


    </div>

    <div class="background-social">
        <div class="container-social">
            <div class="button-container">
                <button>SIGN UP NOW!</button>
            </div>
            

            <ul>
                <li><h3>FOLLOW US</h3></li>
                <li><img src="../assets/footer-facebook.png" alt="logo facebook"></li>
                <li><img src="../assets/footer-twitter.png" alt="logo twitter"></li>
                <li><img src="../assets/footer-youtube.png" alt="logo youtube"></li>
                <li><img src="../assets/footer-pinterest.png" alt="logo pinterest"></li>
                <li><img src="../assets/footer-periscope.png" alt="logo periscope"></li>
            </ul>
        </div>
    </div>



</section>


       
    
</template>


<script>

    export default{
        name: "Footer",
        data(){

            return{
                primaryLinks:[
                    {
                         img: require("../assets/buy-comics-digital-comics.png"),
                        title: "DIGITAL COMICS",
                    },
                    {
                          img: require("../assets/buy-comics-merchandise.png"),
                        title: "DC MERCHANDISE",
                    },
                    {
                         img: require("../assets/buy-comics-subscriptions.png"),
                        title: "SUBSCRIPTION",
                    },
                    {
                          img: require("../assets/buy-comics-shop-locator.png"),
                        title: "COMIC SHOP LOCATOR",
                    },
                    {
                        
                          img: require("../assets/buy-comics-shop-locator.png"),
                        title: "DC POWER VISA",
                    },
                ]
            }
        }
    }

</script>



<style lang="scss" scoped>

    .background-primary{
        background-color: #2196f3;
        z-index: 1;
        position: relative;

        .card-item-link{
            display: flex;
            justify-content: space-around;
            width: 1200px;
            margin: auto;

            .single-card{
                display: flex;
                align-items: center;
                padding: 45px 0;
                color: white;

                .img-single-card{
                    height: 50px;
                    width: 50px;
                    padding: 0px 10px;

                   img{
                       width: 100%;
                       object-fit: contain;
                   }
                }

            }

        }
    }

    .background-footer{
        background-image: url("../assets/footer-bg.jpg");
        background-size: cover;
        // height: 300px;
        // width: 1200px;

        .container-DC-links{
            width: 1200px;
            display: flex;
            margin: auto;
            position: relative;

            .container-all-links{
                display: flex;
                width: 50%;
                flex-wrap:wrap ;
                padding-top: 50px;

                .single-link{
                    width:  calc(100% / 3);

                    h5{
                        color: white;
                        margin: 0;
                    }

                    ul{
                        padding: 0;
                        color: rgb(197, 195, 194);
                        list-style:none;

                        li{
                            padding: 4px;
                        }
                    }
                }
            }

            img{
                position: absolute;
                top: -50px;
                right: 0;
            }
        }
    }

    .background-social{
        background-color: #303030;;
        position: relative;

        .container-social{
            margin: auto;
            display: flex;
            width: 1200px;
            align-content: center;
            justify-content: space-between;
            padding:  28px 0;
            background-color: #303030;
            
            button{
                
                border: solid 2px #2196f3;
                color: white;
                padding: 10px 15px;
                background-color:  #303030;
                font-weight: bold;
            }


            ul{
                list-style:none;
                padding: 0;
                margin: 0;

                li{
                    display:inline-block;
                    padding: 0 12px;
                    vertical-align: middle;

                    h4{
                        margin: 0;
                        color: #0c7dda;
                    }
                }
            }


        }
    }

</style>