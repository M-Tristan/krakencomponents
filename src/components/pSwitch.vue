<template>
    <div :style="style">
        <div :style="buttonStyle" ></div>
    </div>
</template>

<script lang="ts">
import { CSSProperties, defineComponent, ref } from 'vue'

export default defineComponent({
    setup() {
        const style = ref({
            background: `#68BCF8`,
            borderRadius: `100px`,
            width: `100px`,
            height: `60px`,
            display: 'flex',
            alignItems: "center",
        } as CSSProperties)
        const buttonStyle = ref({
            width:'55px',
            height:"55px",
            backgroundColor:"white",
            borderRadius:"50%"
        } as CSSProperties)
        return { style,buttonStyle }
    }
})
</script>

<style scoped>

</style>