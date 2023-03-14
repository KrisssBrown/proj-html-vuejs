<template>
    <div class="bg-section">
        <div class="controls">

        </div>

        <div class="speaker" v-for="speaker in speakers" :key="index">
            <img :src="speaker.imgSrc" >
            <h4>{{ speaker.name }}</h4>
            <p>{{ speaker.job }}</p>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            speakers: [

                {
                    imgSrc: '../assets/speaker-6.jpg',
                    name: 'PATRICK SPENCER',
                    job: "S&P Analyzer"
                },
                {
                    imgSrc: '../assets/speaker-5.jpg',
                    name: 'JANET JONES',
                    job: "NewYork Post's GM"
                },
                {
                    imgSrc: '../assets/speaker-4.jpg',
                    name: 'MICHEAL DOVER',
                    job: "Starbuck's CEO"
                },
                {
                    imgSrc: '../assets/speaker-3.jpg',
                    name: 'ANGELINA HOLY',
                    job: "Maxii's Manager"
                }
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
.bg-section {
    background-color: #F3F3F3;
    height: 500px;
}
</style>