<template>
    <div class= "character-container">
        <div class="inner">
            <img :src="image" :alt="'image of' + name">
            <div class ="name" >{{name}}</div>
            <hr>
            <div class="origin">{{origin}}</div>
            <div class="species">{{species}}</div>
        </div> 
    </div>
</template>

<script>
export default {
    name:'Character',
    props: {
        name: String,
        origin: String,
        species: String,
        image: String
    }
        
}
</script>

<style lang = "scss" scoped>
    .character-container{
        text-align: center;

        .inner{
            padding: 15px;
           
           img {
            border-radius: 50%;
            width: 100%;
            box-shadow: 1px 1px 6px #aaa;
        }
            .name{
                font-size: 24px;
            }
            hr{
                width: 30%;
                margin: 0 auto;
                background: #000;
            }
            .species{
                font-weight: bold;

            }
        }

        
    }
</style>