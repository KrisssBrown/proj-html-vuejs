<template>
    <div class="container">
        <header>
            <h1>RECENT NEWS</h1>
            <p class="all-news serif">Read All News</p>
        </header>

        <main>
            <div class="card" v-for="info in articleInfo" key="i">
                <figure>
                    <img :src="info.imgSrc" alt="">
                    <!-- <span class="sticky-post">
                        <i class="fa fa-bullhorn" aria-hidden="true"></i>
                        STICKY POST
                    </span> -->
                </figure>


                <div class="article-info">
                    <p>{{ info.date }} / {{ info.comments }}</p>
                    <h2>{{ info.title }}</h2>
                </div>

                <div class="article-preview">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Aspernatur nobis, culpa rerum ipsa,
                        necessitatibus veritatis dignissimos quasi nemo repellat nihil magni eaque reprehenderit ipsum minus
                        praesentium impedit! Delectus, saepe corporis?</p>
                </div>

                <a class="serif" href="#">Read More</a>
            </div>
        </main>
    </div>
</template>

<script>
export default {
    data() {
        return {
            articleInfo: [
                {
                    imgSrc: '/recent/1.jpg',
                    date: '03 Dec 2023',
                    comments: '0 Comments',
                    title: 'SEDIAL EIUSMOD TEMPOR'
                },
                {
                    imgSrc: '/recent/2.jpg',
                    date: '03 Dec 2023',
                    comments: '2 Comments',
                    title: 'DONEC LUCTUS IMPERDIET'
                },
                {
                    imgSrc: '/recent/3.jpg',
                    date: '03 Dec 2023',
                    comments: '2 Comments',
                    title: 'MAGNA PARS STUDIORUM'
                }
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
.container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    height: 675px;
    gap: 40px;
}

header {
    display: flex;
    align-items: center;
    justify-content: space-between;

    h1{
        font-size: 18px;
    }
}

main {
    display: flex;
    gap: 30px;
}

// main:first-child::after{
//     content: '/f0a1 STICKY POST';
//     font-family: "Font Awesome 5 Free";
//     height: 10px;
//     width: 10px;
//     color: red;
// }

.card{
    display: flex;
    flex-direction: column;
    gap: 25px;

    .article-info{

        display: flex;
        flex-direction: column;
        gap: 5px;
        p{
            font-size: 10px;
            font-style: italic;
            color: gray;
        }

        h2{
            font-size: 14px;
        }

    }
    .article-preview{
        font-size: 10px;
        color: gray;
    }
}

figure{
    position: relative;
    display: flex;
}

.sticky-post{
    font-size: 8px;
    background-color: #232323;
    color: white;
    padding: 5px;
    font-weight: 700;
}

.serif{
    color: red;
    font-style: italic;
    font-family: serif;
}
</style>