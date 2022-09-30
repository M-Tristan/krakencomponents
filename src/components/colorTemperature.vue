<template>
    <div>
        <div :style="ballStyle"></div>
        <div :style="barStyle">
            <div :style="innerBarStyle"></div>
        </div>
    </div>
</template>

<script lang="ts">
import { CSSProperties, defineComponent, ref } from 'vue'

export default defineComponent({
    setup () {
        const ballStyle = ref({
            width:"475px",
            height:"475px",
            borderRadius:"50%",
            background: `linear-gradient(180deg, rgba(242, 174, 0, 0.93927) 0%, rgba(255, 252, 245, 0.93927) 98.96%)`
        } as CSSProperties)
        const barStyle = ref({
            width:"622px",
            height:"64px",
            borderRadius:"32px",
            background: `#F0F0F0`,
            display:"flex",
            alignItems:"center"
        } as CSSProperties)
        const innerBarStyle = ref({
            marginLeft:"1px",
            width:"422px",
            height:"60px",
            borderRadius:"32px",
            background: `white`
        } as CSSProperties)
        
        return {ballStyle,barStyle,innerBarStyle}
    }
})
</script>

<style scoped>

</style>