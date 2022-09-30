<template>
    <div :style="style">
        <div :style="navigation">
        <div :style="positionStyle"></div>
        </div>
        <div :style="navigation">1x</div>
    </div>
</template>

<script lang="ts">
import { CSSProperties, defineComponent, ref } from 'vue'

export default defineComponent({
    setup() {
        const navigation = ref({
            width:"186px",
            height:"107px",
            backgroundColor:"rgba(0,0,0,0.5)",
            display:"flex",
            position:"relative",
            justifyContent:"center",
            alignItems:"center",
            color:"white"
        } as CSSProperties)
        const style = ref({
            display:"flex",
            justifyContent:"space-around"
        } as CSSProperties)
        const positionStyle = ref({
            position:"absolute",
            top:"10px",
            left:"10px",
            width:"52px",
            height:"36px",
            backgroundColor:"white"
        } as CSSProperties)
        return {navigation,style,positionStyle}
    }
})
</script>

<style scoped>
.sad{
    position: relative;
}
</style>