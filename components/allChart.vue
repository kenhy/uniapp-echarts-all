<template>
    <view>
        <!-- #ifdef H5 || APP-PLUS -->
        <echarts :option="option" style="height: 360px;"></echarts>
        <!-- #endif -->
        <!-- #ifndef H5 || APP-PLUS -->
        <e-charts canvas-id="zphhhhh" :option="option" width="100%" height="360px" />
        <!-- #endif -->
    </view>

</template>

<script>
    import ECharts from '@/components/ECharts';
    import echarts from "@/components/echart/echarts.vue"
    export default {
        components: {
            ECharts,
            echarts
        },
        props:['option'],
        data() {
            return {

            }
        },
        mounted() {
            console.log(this.option)
        },
    }
</script>
