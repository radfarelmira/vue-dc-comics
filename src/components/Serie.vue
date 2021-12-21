<template>
    <div class="single-serie">
        <div class="single-serie-img">
            <img :src="serieObject.thumb" :alt="serieObject.series">
        </div>
        
        <h4>{{serieObject.series}}</h4>
    </div>
</template>

<script>
export default {
    name: 'Serie',
    props: ['serieObject']
}
</script>

<style lang="scss" scoped>
@import '../style/common.scss';
@import '../style/variables.scss';

.single-serie{
    width: calc((100% / 6) - 8px);
    padding: 30px 0;
    margin: 0 4px;

    .single-serie-img{
        width: 180px;
        height: 180px;
        overflow: hidden;
    }

    h4{
        padding: 10px 0;
        font-size: 14px;
        font-weight: 500;
        color: $secondary_color;
    }

}

</style>