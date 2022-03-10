<template>
    <div class="card-wrapper">
        <figure class="series-image">
            <!-- usando le proprietà singolarmente: -->
            <!-- <img :src="image" alt=""> -->
            <!-- oppure usando la proprietà in cui è stato passato tutto l'oggeto del padre: -->
            <img :src="comicsInfo.thumb" alt="">
        </figure>
        <div class="series-info">
            <div class="series-name">
                <!-- {{seriesName}} -->
                {{comicsInfo.series}}
            </div>
            <div class="type">
                <!-- {{seriesType}} -->
                {{comicsInfo.type}}
            </div>
            <div class="price">
                <!-- {{seriesPrice}} -->
                {{comicsInfo.price}}
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'ComicsDC',
        props: [
            'comicsInfo'
            // 'image',
            // 'seriesName',
            // 'seriesPrice',
            // 'seriesType',
        ],
        // potrei anche specificare il tipo di elemento:
        // props: {
        //     comicsInfo: Object,
        // },

        created() {
            // console.log(this.image, this.seriesName);
            console.log(this.comicsInfo);
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
        // potevo anche usare object-fit e object-position, togliendo overflow e height da series-image:
        // width: 100%;
        // display: block;
        // aspect-ratio: 1/1;
        // object-fit: cover;
        // object-position: center;
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
