<template>
    <section class="block">
        <div class="card-item">
            <div class="card-image">
            </div>
            <div class="card-text">
                <div>
                    <span>type</span><span>popular</span>
                </div>
                
                <span>preview</span>
                
            </div>
            <div class="item-price">
                <span>1500$</span>
            </div>
        </div>
    </section>    
</template>

<script>
export default {
    setup() {
        
    },
}
</script>

<style lang="scss" scoped>
.card-item{
    display: grid;
    grid-template-columns: 200px;
    grid-template-rows: 230px 120px 50px;
    grid-template-areas: "image" "text" "price";
    
    font-family: sans-serif;
    border-radius: 18px;
    background: #fff;
    box-shadow: 5px 5px 12px rgba(0,0,0,0.9);
    text-align: center;
    .card-image{
        grid-area: image;
        background: url("../assets/lespaul.jpg");
        border-top-right-radius:12px;
        border-top-left-radius:12px;
        background-size: cover;
        background-position: center;
    }
    .card-text{
        display: flex;
        flex-direction: column;
      
        grid-area: text;
        margin: 20px;
        // span{
        //     display: flex;
        //     justify-content: left;
        // }
    }
    .item-price{
        grid-area: price;
    }
}
</style>