<template>
    <div class="bg">
        <div class="container">
            <header>
                <h1>TICKETS</h1>
            </header>
    
            <main>
                <div class="card">
    
                </div>
            </main>
    
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
.bg{
    background-image: url(/ticket-bg.jpg);
    height: 680px;
    background-repeat: no-repeat;
    background-size: cover;

    .container{
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;

        header{
            text-align: center;
            color: white;
        }
    }
}
</style>