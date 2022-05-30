<template>
    <section class="shop-page">
        <div class="container flex-row">
            <shopMenu/>
            <div class="shop-gallery">
                <itemPreview/>   
                <itemPreview/>   
                <itemPreview/>  
                <itemPreview/>   
                <itemPreview/>   
                <itemPreview/>  
                <itemPreview/>   
                <itemPreview/>   
                <itemPreview/>  
            </div> 
        </div>
    </section>
</template>

<script>
import shopMenu from "../cmps/shop-menu.vue";
import itemPreview from "../cmps/item-preview.vue";
export default {
    
    setup() {},
    components: {
    shopMenu,
    itemPreview
    },
}
</script>

<style lang="scss" scoped>
.shop-page{
    padding-top:  100px;
    .shop-gallery{
        width: 1000px;
        display: grid;
        column-gap: 40px;
        row-gap: 60px;
        grid-template-columns: repeat(auto-fill, minmax(200px, 200px));
        // grid-template-columns: repeat(auto-fill,minmax(,2fr));
    }
}
</style>