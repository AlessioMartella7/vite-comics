<script>
export default {
  data() {
    return {
      
    }
  }
}
</script>

<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="logo-dc-sm">
            </div>

            <div class="navbar">
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
                    </ul>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>

header {
    background-color: #fff;
    margin-top: 1.5rem;
}

.container {
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

ul {
    height: 140px;
    display: flex;
    align-items: center;
    gap: 2rem;

    li{
        display: flex;
        align-items: center;
        height: 100%;
        &:hover {
            border-bottom: 3px solid #0C7CEC;
        }
    }
}

a {
    text-transform:uppercase;
    color: #1C1C1C;

    &:hover {
        color: #0C7CEC;
        }
}
</style>