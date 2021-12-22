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
@import '../style/mixin.scss';

.single-serie{
    width: calc(100% / 6);
    padding: 30px 8px;

    .single-serie-img{
        width: 100%;
        height: 200px;
        overflow: hidden;
            img{
                @include image-fit;
            }
    }

    h4{
        padding: 10px 0;
        font-size: 14px;
        font-weight: 500;
        color: $secondary_color;
    }

}

</style>