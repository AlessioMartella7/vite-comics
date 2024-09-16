<script>
export default {
  data() {
    return {
      
    }
  }
}
</script>

<template>
   <div id="footer-top">
        <div class="container">
            <div class="footer-links">
                <div class="col left-col">
                    <section id="dc-comics">
                        <h5>DC COMICS</h5>
                        <ul>
                            <li><a href="#">link</a></li>
                            <li><a href="#">link</a></li>
                            <li><a href="#">link</a></li>
                            <li><a href="#">link</a></li>
                            <li><a href="#">link</a></li>
                            <li><a href="#">link</a></li>
                            <li><a href="#">link</a></li>
                        </ul>
                    </section>

                    <section id="shop">
                        <h5>SHOP</h5>
                        <ul>
                            <li><a href="#">link</a></li>
                            <li><a href="#">link</a></li>
                        </ul>
                    </section>
                </div>


                <div class="col middle-col">
                    <section id="dc-comics">
                        <h5>DC</h5>
                        <ul>
                            <li><a href="#">link</a></li>
                            <li><a href="#">link</a></li>
                            <li><a href="#">link</a></li>
                            <li><a href="#">link</a></li>
                            <li><a href="#">link</a></li>
                            <li><a href="#">link</a></li>
                            <li><a href="#">link</a></li>
                            <li><a href="#">link</a></li>
                            <li><a href="#">link</a></li>
                            <li><a href="#">link</a></li>
                            <li><a href="#">link</a></li>
                        </ul>
                    </section>
                </div>

                <div class=" col right-col">
                    <section id="sites">
                        <h5>SITES</h5>
                        <ul>
                            <li><a href="#">link</a></li>
                            <li><a href="#">link</a></li>
                            <li><a href="#">link</a></li>
                            <li><a href="#">link</a></li>
                            <li><a href="#">link</a></li>
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
    height: 500px;
}

.container {
    display: flex;
    justify-content: space-between;
    padding-top: 2rem;
}

.footer-links {
    width: 30%;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-content: center;
}

col {
    width: calc(100%/3);
}

h5 {color: #fff;
    font-size: 1.5rem;
}

li {
    margin: 5px 0;
    a {
        color: gray;
    }
}

</style>