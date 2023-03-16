<template>
    <div>
        <div class="bg">
            <div class="container">
                <div class="container-sm">
                    <h1>LOCATION</h1>
                    <h3>GD BUILDING, GRAND CONFERENCE ROOM</h3>

                    <div class="address">
                        <i class="fa fa-location-arrow" aria-hidden="true"></i>
                        <p>11 GD Building, River Mall, New york, USA 8879</p>
                    </div>

                    <a href="#">Check for Accomodations Here</a>

                    <div class="contact">
                        <div class="number">
                            <i class="fa fa-phone" aria-hidden="true"></i>
                            <p>+1-112-222-3344</p>
                        </div>
                        <div class="mail">
                            <i class="fa fa-envelope" aria-hidden="true"></i>
                            <p>Contact@TheKeynoteTheme.com</p>
                        </div>
                    </div>

                </div>


            </div>
        </div>

    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.bg {
    height: 445px;
    background-image: url(/location-bg.jpg);
    margin-top: 10px;
    background-repeat: no-repeat;
    background-size: cover;
}

.container {
    height: 100%;
}

.container-sm {
    max-width: 800px;
    margin: 0 auto;
    color: white;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 100%;
    gap: 30px;
}

a{
    color: rgb(255, 41, 41);
}
.address {
    display: flex;
    align-items: center;
    gap: 10px;
}

.h1 {
    font-size: 26px;
}

h3 {
    font-size: 22px;
}

.contact {
    display: flex;
    gap: 40px;
    border-top: 2px solid;
}

.number, .mail {
    display: flex;
    align-items: center;
    gap: 10px;
    padding-top: 10px;
}
</style>