<template>
    <div class="bg-section">
        <div class="countdown-container">
            <ul class="cards">
                <li class="card" style="opacity: 0.7;">
                    <h1><strong>3399</strong></h1>
                    <p>DAYS</p>
                </li>
                <li class="card" style="opacity: 0.65;">
                    <h1><strong>17</strong></h1>
                    <p>HOURS</p>
                </li>
                <li class="card" style="opacity: 0.6;">
                    <h1><strong>28</strong></h1>
                    <p>MINS</p>
                </li>
                <li class="card" style="opacity: 0.55;">
                    <h1><strong>17</strong></h1>
                    <p>SECS</p>
                </li>
            </ul>

            <p class="subs">SUBSCRIBE FOR UPDATES</p>

            <div class="input-section">
                <input class="text" type="text" placeholder="Please fill your email">

                <button class="btn">SUBSCRIBE</button>
            </div>
        </div>

    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.bg-section {
    background-image: url(/coutdown-bg1.jpg);
    height: 495px;

    .countdown-container {
        max-width: 800px;
        margin: 0 auto;
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 30px;
    }
}

.subs {
    font-size: 15px;
    font-weight: 600;
}

.cards {
    display: flex;
    justify-content: center;
    gap: 40px;
    align-items: center;
    // height: 100%;
    color: white;



    .card {
        background-color: black;
        padding: 29px 53px;
        border-radius: 7px;
        display: flex;
        flex-direction: column;
        gap: 20px;
        align-items: center;

        h1 {
            font-size: 38px;
            font-weight: 800;
            opacity: 1;
        }

        p {
            font-size: 13px;
            opacity: 1;

        }
    }

}

.input-section {
    display: flex;
    gap: 14px;

    .text {
        padding: 10px 5px;
        padding-right: 120px;
        border: 0;
    }

    .btn {
        padding: 10px 25px;
        font-weight: 700;
        color: white;
        background-color: red;
        border: 0;
    }
}
</style>