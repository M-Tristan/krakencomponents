<template>
    <div :style="style">
        <div :style="innerStyle">

</div>
    </div>
</template>

<script lang="ts">
import { CSSProperties, defineComponent, ref } from 'vue'

export default defineComponent({
    setup () {
        const style=ref({
            width:"270px",
            height:"270px",
            borderRadius:'50%',
            backgroundColor:"rgba(0, 0, 0, 0.5)",
            border: `2px solid #FFFFFF`,
            display:"flex",
            justifyContent:"center",
            alignItems:"center"
        } as CSSProperties)
        const innerStyle=ref({
            width:"150px",
            height:"150px",
            borderRadius:'50%',
            // backgroundColor:"rgba(0, 0, 0, 0.5)",
            border: `2px solid #FFFFFF`
        } as CSSProperties)
        return {style,innerStyle}
    }
})
</script>

<style scoped>

</style>