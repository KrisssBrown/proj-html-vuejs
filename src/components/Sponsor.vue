<template>
    <div class="bg">
        <div class="container">
            <h1 class="title">SPONSOR</h1>
            <p class="sponsor-text">
                Lorem ipsum dolor, sit amet consectetur adipisicing elit. Autem, facilis?
            </p>
            <ul class="sponsor">
                <li class="sponsor-item" v-for="src in sponsorSrc" :key="i">
                    <a href="#">
                        <img :src="src" alt="">
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            sponsorSrc: [
                '/sponsor/banner-1.jpg',
                '/sponsor/banner-2.jpg',
                '/sponsor/banner-3.jpg',
                '/sponsor/banner-4.jpg',
                '/sponsor/banner-5.jpg',
                '/sponsor/banner-6.jpg',
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
.bg{
    background-color: #F6F6F6;
    height: 475px;

    .container{
        height: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        gap: 25px;

        .sponsor-text{
            color: gray;
            width: 500px;
        }
        .sponsor{
            display: flex;
            align-items: center;
            gap: 37px;
            padding-top: 30px;

            
        }
    }
}
</style>