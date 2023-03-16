<template>
    <main class="bg">
        <div class="container">
            <ul class="section">
                <li class="about-us">
                    <h6>ABOUT US</h6>
                    <ul class="item-list">
                        <li>
                            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ab sit fuga obcaecati corporis,
                            molestias laboriosam?
                        </li>
                        <li class="social">
                            <a href="#">
                                <i class="fa-brands fa-square-facebook"></i>
                            </a>
                            <a href="#">
                                <i class="fa-brands fa-square-twitter"></i>
                            </a>
                            <a href="#">
                                <i class="fa-brands fa-linkedin"></i>
                            </a>
                            <a href="#">
                                <i class="fa-brands fa-square-google-plus"></i>
                            </a>
                            <a href="#">
                                <i class="fa-brands fa-square-pinterest"></i>
                            </a>
                            <a href="#">
                                <i class="fa-brands fa-flickr"></i>
                            </a>
                        </li>
                    </ul>
                </li>
                <li class="recent-news">
                    <h6>RECENT NEWS</h6>
                    
                    <div class="news-list">
                        <a href="#">
                            <i class="fa fa-chevron-right" aria-hidden="true"></i>
                            <p>SEM PORTA MOLLIS PARTURIENT</p>
                        </a>
                        <a href="#">
                            <i class="fa fa-chevron-right" aria-hidden="true"></i>
                            <p>NULLAM LOREM MATTIS PURUS</p>
                        </a>
                        <a href="#">
                            <i class="fa fa-chevron-right" aria-hidden="true"></i>
                            <p>NIBH SEM SIT ULLAMCORPER</p>
                        </a>
                        <a href="#">
                            <i class="fa fa-chevron-right" aria-hidden="true"></i>
                            <p>DONEC LUCTUS IMPERDIET</p>
                        </a>
                        <a href="#">
                            <i class="fa fa-chevron-right" aria-hidden="true"></i>
                            <p>MAGNA PARS STUDIORUM</p>
                        </a>
                    </div>
                </li>
                <li class="get-your-seat">
                    <h6>GET YOUR SEAT!</h6>
                    <div>
                        <p>Book for your seat before it's too late. We provide variety of ticket options.</p>
                        <button href="#">CHECK OUT TICKETS!</button>
                    </div>
                </li>
                <li class="gallery">
                    <div class="title">
                        <h6>GALLERY FROM LAST YEAR</h6>
                    </div>
                    <div class="gallery-items">
                        <a href="#" v-for="img in gallery" :key="i">
                            <img :src="img" alt="">
                        </a>
                    </div>
                </li>
            </ul>
        </div>
    </main>
    <footer>

    </footer>
</template>

<script>
export default {
    data() {
        return {
            gallery:[
                '/gallery/1.jpg',
                '/gallery/2.jpg',
                '/gallery/3.jpg',
                '/gallery/4.jpg',
                '/gallery/5.jpg',
                '/gallery/6.jpg',
                '/gallery/7.jpg',
                '/gallery/8.jpg',
                '/gallery/9.jpg',
                '/gallery/10.jpg',
                '/gallery/11.jpg',
                '/gallery/12.jpg',
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
.bg {
    background-color: #212121;
}

.section {
    display: flex;
    color: white;
    gap: 50px;
    padding: 50px 0;

    li {
        flex-basis: calc(100% / 4);

        h6{
            font-size: 14px;
        }
    }

    .about-us {
        display: flex;
        flex-direction: column;
        gap: 35px;

        .item-list {
            display: flex;
            flex-direction: column;
            gap: 30px;
        }

        .social {
            display: flex;
            gap: 5px;

            i{
                font-size: 22px;
            }
        }
    }

    .recent-news{
        display: flex;
        flex-direction: column;
        gap: 35px;

        .news-list{
            display: flex;
            flex-direction: column;
            gap: 10px;

            a{
                display: flex;
                align-items: center;
                gap: 5px;

                p{
                    font-size: 11px;
                }
            }
        }
    }

    .get-your-seat{
        display: flex;
        flex-direction: column;
        gap: 35px;

        div{
            display: flex;
            flex-direction: column;
            gap: 15px;

            p{
                font-size: 12px;
            }

            button{  
                
                background-color: red;
                font-size: 10px;
                font-weight: 600;
                padding: 15px;
                color: white;
                border: 0;
                align-self: flex-start;
                cursor: pointer;

            }
        }
    }

    .gallery{
        display: flex;
        flex-direction: column;
        gap: 30px;

        .gallery-items{
            display: grid;
            grid-template-columns: repeat(4,1fr);
            gap: 10px;
            
            img{
                display: block;
            }
        }
    }
}
</style>