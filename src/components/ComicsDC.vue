<template>
    <div class="card-wrapper">
        <figure class="series-image">
            <img :src="image" alt="">
        </figure>
        <div class="series-info">
            <div class="series-name">
                {{seriesName}}
            </div>
            <div class="type">
                {{seriesType}}
            </div>
            <div class="price">
                {{seriesPrice}}
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'ComicsDC',
        props: [
            'image',
            'seriesName',
            'seriesPrice',
            'seriesType'
        ],

        created() {
            console.log(this.image, this.seriesName)
        }
    }
</script>

<style scoped lang="scss">

.card-wrapper{
    color: white;
    font-size: 14px;
}

.series-image{
    color: white;
    overflow: hidden;
    height: 169px; 
    margin-bottom: 10px;
    
    img{
        width: 100%;
    }
}

.series-info{
    
    .series-name, .type, .price{
        margin-bottom: 7px;
    }

    .series-name{
        text-transform: uppercase;
        font-weight: 500;
    }
    
    .type{
        color: #acacac;
    }
    
    .price{
        color: #55BA59;
    }
}



</style>
