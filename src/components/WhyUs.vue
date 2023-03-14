<template>
    <div>
        <ul class="container about">
            <li class="who-we-are">
                <i class="fa fa-trophy" aria-hidden="true"></i>
                <div class="about-text">
                    <h1>WHO WE ARE</h1>
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Perferendis quibusdam rerum aspernatur
                        repudiandae cupiditate voluptates incidunt deserunt porro eligendi maxime.</p>
                    <a class="learn-more" href="@">Learn More</a>
                </div>
            </li>
            <li class="what-we-do">
                <i class="fa-solid fa-bolt-lightning"></i>
                <div class="about-text">
                    <h1>WHAT WE DO</h1>
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Perferendis quibusdam rerum aspernatur
                        repudiandae cupiditate voluptates incidunt deserunt porro eligendi maxime.</p>
                    <a class="learn-more" href="@">Learn More</a>
                </div>
            </li>
            <li class="why-us">
                <i class="fa-solid fa-question"></i>
                <div class="about-text">
                    <h1>WHY US?</h1>
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Perferendis quibusdam rerum aspernatur
                        repudiandae cupiditate voluptates incidunt deserunt porro eligendi maxime.</p>
                    <a class="learn-more" href="@">Learn More</a>
                </div>
            </li>
        </ul>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.about {
    display: flex;
    height: 230px;
    padding: 40px 0;
    gap: 30px;

    li {
        display: flex;
        gap: 30px;

        .about-text{
            display: flex;
            flex-direction: column;
            gap: 10px;
        }

        i {
            font-size: 26px;
            color: gray;
        }

        h1 {
            font-size: 13px;
            line-height: 26px;
        }

        p{
            color: gray;
            font-size: 10px;
        }

        a{
            color: red;
            font-style: italic;
        }
    }
}
</style>