<script>
export default {
  data() {
    return {
        dcComicLinks: [
        {
            name: 'Characters'
        },
        {
            name: 'Comics'
        },
        {
            name: 'Covies'
        },
        {
            name: 'Tv'
        },
        {
            name: 'Games'
        },
        {
            name: 'Collectibles'
        },
        {
            name: 'News'
        },
      ],
        shopLinks: [
        {
            name: 'Shop DC'
        },
        {
            name: 'Shop DC Collectibles'
        },
      ],
        dcLinks: [
        {
            name: 'Terms Of Use'
        },
        {
            name: 'Privacy policy(New)'
        },
        {
            name: 'Ad Choices'
        },
        {
            name: 'Advetising'
        },
        {
            name: 'Jobs'
        },
        {
            name: 'Subscriptions'
        },
        {
            name: 'Talent Workshop'
        },
        {
            name: 'CPSC Certificates'
        },
        {
            name: 'Ratings'
        },
        {
            name: 'Shop Help'
        },
        {
            name: 'Contact Us'
        }
      ],
        sitesLinks: [
        {
            name: 'DC'
        },
        {
            name: 'MAD Magazine'
        },
        {
            name: 'DC Kids'
        },
        {
            name: 'DC Universe'
        },
        {
            name: 'DC Power Visa'
        },
      ],
      iconsList: [
        {
            imgUrl: 'buy-comics-digital-comics.png',
            name: 'digital-comics'
        },
        {
            imgUrl: 'buy-comics-merchandise.png',
            name: 'dr merchandise'
        },
        {
            imgUrl: 'buy-comics-subscriptions.png',
            name: ' subscription'
        },
        {
            imgUrl: 'buy-comics-shop-locator.png',
            name: 'comic shop locator'
        },
        {
            imgUrl: 'buy-dc-power-visa.svg',
            name: 'dc power visa'
        },
      ]
    }
  },
  methods: {
    getImageUrl (imagePath){
        return new URL (`../assets/img/${imagePath}`, import.meta.url).href;
    }
  },
}
</script>

<template>
    <div id="footer-top">
       <div class="banner-footer-top">
        
            <div class="icons-container" v-for="(icon,index) in iconsList" :key="index"> 
                <img :src="getImageUrl(icon.imgUrl)" :alt="icon.name">
                <p>{{ icon.name }}</p>
            </div>
       
       </div>
        <div class="container">
            <div class="footer-links">
                <div class="col left-col">
                    <section id="dc-comics">
                        <h5>DC COMICS</h5>
                        <ul>
                            <li v-for="link in dcComicLinks">
                                <a href="#">{{link.name}}</a>
                            </li>

                            
                        </ul>
                    </section>

                    <section id="shop">
                        <h5>SHOP</h5>
                        <ul>
                            <li v-for="link in shopLinks">
                                <a href="#">{{link.name}}</a>
                            </li>
                        </ul>
                    </section>
                </div>


                <div class="col middle-col">
                    <section id="dc-comics">
                        <h5>DC</h5>
                        <ul>
                            <li v-for="link in dcLinks">
                                <a href="#">{{link.name}}</a>
                            </li>
                        </ul>
                    </section>
                </div>

                <div class=" col right-col">
                    <section id="sites">
                        <h5>SITES</h5>
                        <ul>
                            <li v-for="link in sitesLinks">
                                <a href="#">{{link.name}}</a>
                            </li>
                        </ul>
                    </section>
                </div>  
            </div>
            <div class="logo">
                <img src="../assets/img/dc-logo-bg.png" alt="logo-dc-lg">
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>


#footer-top {
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    height: 540px;
    padding-top: 6rem;
    position: relative;
    
    .banner-footer-top {
        height: 160px;
        background-color: #0C7CEC;
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        padding: 0 5rem;
        
        .icons-container{
            display: flex;
            align-items: center;
           
        }
        img {
            height: 65px;
        }
         img:last-child {
            width: 50px;
        }
        p {
            color: #fff;
            margin-left: 2rem;
            font-weight: 600;
            color: #fff;
            text-transform: uppercase;

        }
    
    }
}

.container {
    display: flex;
    justify-content: space-between;
    padding-top: 1rem;
}

.footer-links {
    margin-top: 5rem;
    display: flex;
    justify-content: space-between;
    align-content: center;
}

col {
    width: calc(100%/3);
}

.left-col,
.middle-col{
    margin-right: 3.5rem;
}

h5 {color: #fff;
    font-size: 1.5rem;
}

li {
    margin: 5px 0;
    a {
        color:gray;
    }
}

</style>