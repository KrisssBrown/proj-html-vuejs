<template>
    <div class="container">
        <header>
            <div class="title-info">
                <h1>PROGRAM</h1>
                <p>This conference run through all 4 days from 23-26 May 2016. <br>
                    We also provide free lunch and coffee break in each day.</p>
            </div>

            <p class="full-prog">View Full Program</p>
        </header>
        <main>
            <ul class="calendar">
                <li class="calendar-item" v-for="item in calendar" :key="i">
                    <h3>{{ item.day }}</h3>
                    <p>{{ item.date }}</p>
                </li>
                <li class="calendar-item">

                </li>
            </ul>
            <div class="program-body">
                <ul class="info">

                    <li>
                        <i class="fa fa-clock-o" aria-hidden="true"></i>
                        <p>09:00 - 10:30</p>
                    </li>
                    <li>
                        <i class="fa fa-location-arrow" aria-hidden="true"></i>
                        <p>ROOM A</p>
                    </li>
                    <li>
                        <i class="fa fa-user" aria-hidden="true"></i>
                        <p class="name">LAURENCE FRANCIS</p>
                    </li>



                </ul>
                <div class="details">
                    <h2>WELCOMING AND INTRODUCTION</h2>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eaque quod blanditiis eius nihil ad magni labore minima exercitationem, optio vero libero doloribus esse aliquam commodi rem expedita, quia iusto ipsa voluptas? Dolorem nobis eaque est?</p>
                    <img src="../assets/speaker-8-150x150.jpg" width="45" alt="picture">
                </div>
            </div>
        </main>

    </div>
</template>

<script>
export default {
    data() {
        return {
            calendar: [
                {
                    day: 'DAY 1',
                    date: '23 May 2023'
                },
                {
                    day: 'DAY 2',
                    date: '24 May 2023'
                },
                {
                    day: 'DAY 3',
                    date: '25 May 2023'
                },
                {
                    day: 'DAY 4',
                    date: '26 May 2023'
                },
                {
                    day: 'DAY 5',
                    date: '27 May 2023'
                }
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
.container {
    height: 665px;
    display: flex;
    flex-direction: column;
    gap: 30px;
    justify-content: center;
}

header {
    display: flex;
    justify-content: space-between;
    align-items: center;

    .title-info {
        display: flex;
        align-items: center;
        gap: 80px;

        p {
            font-size: 12px;
            color: gray;
        }

        h1 {
            font-size: 27px;
        }
    }

    .full-prog {
        font-size: 11px;
        color: red;
        font-style: italic;
        font-family: serif;
    }
}

.calendar {
    display: flex;

    .calendar-item {
        flex-basis: calc(100% /6);
        background-color: red;
        color: white;
        height: 70px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        padding-left: 15px;
        border-right: 1px solid #D52B0F;
    }
}

.program-body {
    background-color: #F7F7F7;
    display: flex;
    height: 285px;
    // padding: 40px;

    .info {
        display: flex;
        flex-direction: column;
        width: 300px;
        gap: 15px;
        padding: 40px;
        

        li {
            display: flex;
            align-items: center;
            
            gap: 20px;
            color: gray;

            i{
                font-size: 15px;
            }

            p{
                font-size: 10px;
            }

            .name{color: red;}
        }
    }

    .details{

        display: flex;
        flex-direction: column;
        gap: 35px;
        padding-top: 40px;
        


        h2{
            font-size: 17px;
            font-weight: 400;
        }

        p{
            font-size: 10px;
        }
    }
}
</style>