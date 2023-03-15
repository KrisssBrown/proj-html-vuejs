<template>
    <div class="bg-section">
        <div class="container">
            <div class="section-header">
                <div class="title">
                    <h1>SPEAKERS</h1>
                </div>
                <div class="controls">
                    <i class="fa fa-chevron-left" aria-hidden="true"></i>
                    <i class="fa fa-chevron-right" aria-hidden="true"></i>
                </div>
            </div>

            <div class="speakers">
                <div class="speaker-el" v-for="speaker in speakers" :key="index">
                    <img :src="speaker.imgSrc">
                    <h4>{{ speaker.name }}</h4>
                    <p>{{ speaker.job }}</p>
                </div>
            </div>

        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            speakers: [

                {
                    imgSrc: '/speakers/speaker-6.jpg',
                    name: 'PATRICK SPENCER',
                    job: "S&P Analyzer"
                },
                {
                    imgSrc: '/speakers/speaker-5.jpg',
                    name: 'JANET JONES',
                    job: "NewYork Post's GM"
                },
                {
                    imgSrc: '/speakers/speaker-4.jpg',
                    name: 'MICHEAL DOVER',
                    job: "Starbuck's CEO"
                },
                {
                    imgSrc: '/speakers/speaker-3.jpg',
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

    .container {
        display: flex;
        flex-direction: column;
        justify-content: space-evenly;
        height: 100%;
        // gap: 20px;
    }
}

.section-header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    
    h1{
        font-size: 25px;
    }

    .controls {

        display: flex;
        gap: 5px;

        .fa-chevron-left,
        .fa-chevron-right {
            background-color: red;
            color: white;
            aspect-ratio: 1;
            font-size: 8px;
            padding: 10px 12px;
            border-radius: 3px;

        }
    }
}

.speakers {
    display: flex;
    justify-content: space-between;
    // gap: 30px;

    .speaker-el {
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 6px;


        img {
            width: 250px;
            border-radius: 6px;
        }

        h4 {
            font-size: 10px;
        }

        p {
            font-size: 8px;
            font-style: italic;
            color: gray;
        }
    }

}
</style>





089014043042800
