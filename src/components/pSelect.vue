<template>
    <div :style="style">
<div>Mode</div>
<div>cool
    <img src="../assets/vector.png">
</div> 
    </div>
</template>

<script lang="ts">
import { CSSProperties, defineComponent, ref } from 'vue'

export default defineComponent({
    setup () {
        
        const style = ref({
            width:"100%",
            height:"98px",
            backgroundColor:"#FAFAFA",
            borderRadius:"8px",
            display:"flex",
            alignItems:"center",
            justifyContent:'space-between'
        } as CSSProperties)
        return {style}
    }
})
</script>

<style scoped>
/* .{
    justify-content: space-between;
} */
</style>