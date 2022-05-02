<template>
    <div class="home_container">
        <div class="left_container">
            <p>
                I'M WINGMAN
            </p>
            <h2>
                Peace On Earth A Wonderful Wish But No Way
            </h2>
            <p>
                Success isn't overnight. It's when everyday you get a little better than the day before. It all adds up.
            </p>
            <button>
                Get Started For Free
                <i class="fa-solid fa-right-long"></i>
            </button>
        </div>
        <div class="right_container">
            <img src="../assets/img/home-movation-hero-image.png" alt="">
        </div>
    </div>
</template>

<script>
    export default {
        name: 'HomePageComp',
        props: {}
    }
</script>

<style scoped lang="scss">
    .home_container {
        display: flex;
        align-items: center;
        padding: 0 15%;
        margin: 50px 0;
        height: 600px;
    }

    .right_container {
        background-image: url('../assets/img/home-movation-shape-face.png');
        background-repeat: no-repeat;
        background-size: contain;
        img{
            height: 100%;
        }
        height: 100%;
    }

    .left_container {
        margin-right: 10%;
        height: 100%;
        >* {
            margin-bottom: 30px;
        }
        
        p:first-of-type {
            font-weight: 600;
        }

        p:nth-of-type(2) {
            font-weight: 100;
        }

        h2 {
            font-size: 3rem;
        }

        button {
            padding: 15px 40px;
            border-radius: 10px;
            border-color:#20ad96;
            background: #20ad96;
            color: white;
            font-weight: bold;
            &:hover{
                
                background:#3f3a64;
                border-color: #3f3a64;
                cursor: pointer;
            }
                
        }
    }
</style>