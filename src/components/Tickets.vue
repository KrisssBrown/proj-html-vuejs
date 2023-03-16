<template>
    <div class="bg">
        <div class="container">
            <header>
                <h1>TICKETS</h1>
            </header>

            <main class="cards">
                <div class="card" v-for="info in cardInfo" :key="i">
                    <header class="card-header">
                        <h1 class="packName">{{info.packName}}</h1>
                        <p class="price">{{info.price}}</p>
                    </header>

                    <main class="card-body">
                        <p>{{info.access}}</p>
                        <p>Coffe Break</p>
                        <p>Lunch (International Buffet)</p>
                        <p>Document Sheets</p>
                        <p>{{info.voucher}}</p>
                    </main >

                    <footer class="card-footer">
                        <a href="#">BOOK NOW</a>
                    </footer>

                </div>
            </main>

        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            cardInfo: [
                {
                    packName: 'ONE DAY PASS' ,
                    price: 'Free',
                    access: 'One Day Access',
                    voucher: '50USD Voucher For Next Event'
                },
                {
                    packName: 'FOUR DAY PASS',
                    price: '750.00 USD',
                    access: 'Four Day Access',
                    voucher: '100USD Voucher For Next Event'
                },
                {
                    packName: 'Two DAY PASS',
                    price: '580.00 USD',
                    access: 'Two Day Access',
                    voucher: '70USD Voucher For Next Event'
                },
                
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
.bg {
    background-image: url(/ticket-bg.jpg);
    height: 680px;
    background-repeat: no-repeat;
    background-size: cover;

    .container {
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        gap: 40px;

        header {
            text-align: center;
            color: white;
        }

        .cards{
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 35px;
            width: 100%;
        }

        .card-header{
            background-color: #E9E9E9;

            .packName{
                color: black;
                font-size: 14px;
            }

            .price{
                color: red;
                font-size: 12px;
            }
        }

        .card-body{
            background-color: white;
            font-style: italic;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            font-size: 15px;
            gap: 10px;
            padding: 43px 27px;
            
        }

        .card-footer{
            text-align: center;
            color: white;
            background-color: red;
            font-size: 11px;
            font-weight: 800;
        }

        .card-footer:hover{
            color: salmon;
        }

        .card-header{
            padding: 25px;
        }

        .card-footer{
            padding: 10px;
        }
    }
}
</style>