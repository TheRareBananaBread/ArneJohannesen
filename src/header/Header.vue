<template>
    <div class="top-bar">
        <div class="main">
            <a class="logo__btn" href="/">
                Arne Johannesen
            </a>
            <app-nav></app-nav>
        </div>
    </div>
</template>

<script>
import Nav from "./Nav.vue";
export default {
    data: function() {
        return{

        }
    },
    methods: {
        
    },
    components: {
        "app-nav": Nav
    }
}
</script>


<style lang="scss">
    .logo__btn{
        background: none;
        border: none;
        margin-left: 100px;
        color: white;
        text-decoration: none;
        font-size: 50px;
        
        &:hover{
            cursor: pointer;
        }
    }

    .logo__img{
        color: black;
        background: black;
        width: 400px;
        padding-top: 5px;
        //height: 100%;
        height: -moz-fit-content;
    }

    .top-bar{
        background: black;
        display: flex;
        flex-direction: row;
        justify-content: center;
    }

    .main{
        //display: flex;
        width: 100%;
    }

    .nav{
        padding-left: 100px;
    }

    /* Dropdown Arrow */
    i{
        border: solid white;
        border-width: 0 3px 3px 0;
        display: inline-block;
        padding: 3px;
        margin-left: 5px;
        
        &--down {
            transform: rotate(45deg);
            -webkit-transform: rotate(45deg);
        }
        
        &--right {
            transform: rotate(-45deg);
            -webkit-transform: rotate(-45deg);
        }
    }
</style>
