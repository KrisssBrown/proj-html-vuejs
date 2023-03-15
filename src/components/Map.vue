<template>
    <div>
        <div class="map">
            <img :src="map" v-for="map in imgMap" :key="index">
            <!-- <div class="map-type">
                <button>
                    Map
                </button>
                <button>
                    Satellite
                </button>
            </div>
            <div class="zoom">
                <button>+</button>
                <button>-</button>
            </div> -->
        </div>

    </div>
</template>

<script>
export default {
    data() {
        return {
            imgMap: [
                '/map/vt (17).png',
                '/map/vt (11).png',
                '/map/vt (1).png',
                '/map/vt (5).png',
                '/map/vt (4).png',
                '/map/vt (9).png',
                '/map/vt (20).png',
                '/map/vt (13).png',
                '/map/vt (12).png',
                '/map/vt (2).png',
                '/map/vt.png',
                '/map/vt (3).png',
                '/map/vt (15).png',
                '/map/vt (18).png',
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
.map {
    display: flex;
    flex-wrap: wrap;
    // max-width: 100%;
    // grid-template-columns: repeat(7);

    img {
        display: block;
        flex-basis: calc(100% / 7);
    }

    // .map-type, .zoom{
    //     display: flex;
    // }

    // button{
    //     border: 1px solid;
    //     padding: 5px;
    //     background-color: red;
    //     color: gray;
    //     font-size: 14px;
    // }

    // .zoom{

    //     button{
    //         padding: 5px 9px ;
    //     }
    // }
}

</style>