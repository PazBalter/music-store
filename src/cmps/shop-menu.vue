<template>
    <section class="left-menu">
            <div class="flex-centered-column">
                <div class="items-sort"><input type="text"></div>
                <ul>
                    <li>All</li>
                    <li>Guitars</li>
                    <li>Amps</li>
                    <li>Pedals</li>
                    <li>Others</li>
                </ul>
            </div>
    </section>
</template>

<script>
export default {
    setup() {},
}
</script>

<style lang="scss" scoped>
    .left-menu{
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: left;
        width: 250px;
        margin-right:40px;
        
        .items-filter{
            padding: 16px;
        }
        ul{
        font-weight: 500;
        list-style: none;
        text-decoration: none;
        display: flex;
        flex-direction: column;
        }

        li{
            border-bottom: 1px solid rgba($color: #000000, $alpha: .1);
            padding: 16px;
            cursor: pointer;
            transition: 0.4s ease all;
            &:hover{
                color: red;
                border-bottom: solid 3px ;
                border-color: red;
                background-color: #cbc8c8
            }
        }
    }
</style>