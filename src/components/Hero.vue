<template>
    <div class="bg-container">
        <div class="container">
            <div class="hero-container">
                <p>CONFERENCE ON</p>
                <p><strong>SOCIAL NETWORK</strong></p>
                <img src="/1-item-2.jpg">
                <ul>
                    <li><strong>
                            23 - 26 MAY 2019
                        </strong></li>
                    <li><strong>
                            /
                        </strong></li>
                    <li><strong>
                            SAN FRANCISCO
                        </strong></li>
                    <li><strong>
                            /
                        </strong></li>
                    <li><strong>
                            8 SPEAKERS
                        </strong></li>
                </ul>

                <button class="register-btn">REGISTER ONLINE</button>
            </div>
        </div>
    </div>
</template>

<!-- ************************************************************************** -->

<script>

export default {

    data() {
        return {

        }
    },
}
</script>

<!-- ************************************************************************** -->

<style lang="scss" scoped>
.bg-container {
    background-image: url(/slider-1-bg.jpg);
    height: 600px;
    object-fit: cover;
    background-repeat: no-repeat;
    object-position: center;
}

.container {
    height: 100%;
}

.hero-container {
    max-width: 900px;
    margin: 0 auto;
    color: white;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100%;
    gap: 10px;
}

.register-btn {
    font-weight: 600;
    font-size: 14px;
    padding: 20px 38px;
    border-radius: 5px;
    color: white;
    background-color: red;
    border: 0;
    margin-top: 24px;
}

.hero-container p {
    font-size: 55px;

    strong {
        font-size: 85px;
    }
}

.hero-container ul {
    display: flex;
    gap: 20px;
    padding: 10px;
}
</style>