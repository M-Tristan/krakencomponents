<template>
    <div style="position:relative">
        <div :style="style"></div>
        <div :style="bgstyle"></div>
        <img :style="imgStyle" src="../assets/rollershutter.png">
    </div>
</template>

<script lang="ts">
import { CSSProperties, defineComponent, ref } from 'vue'

export default defineComponent({
    setup() {

        const style = ref({
            width: "622px",
            height: "14px",
            backgroundColor: "#ECECEC",
            borderRadius: "20px"
        } as CSSProperties)
        const bgstyle = ref({
            width: "514px",
            height: "454px",
            border: `20px solid #F8F8F8`,
            borderRadius: `4px`
        } as CSSProperties)
        const imgStyle = ref({
            position:'absolute',
            top:"20px",
            left:0
        } as CSSProperties)
        return { style, bgstyle,imgStyle }
    }
})
</script>

<style scoped>

</style>