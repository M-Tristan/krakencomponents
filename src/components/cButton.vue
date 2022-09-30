<template>
    <div :style="style">
        <slot></slot>
    </div>
</template>

<script lang="ts">
import { CSSProperties, defineComponent, ref } from 'vue'

export default defineComponent({
    setup() {
        const style = ref({
            boxSizing: `border-box`,
            width: `80px`,
            height: `80px`,
            display: 'flex',
            justifyContent: 'center',
            alignItems: "center",
            border: `1.2px solid #C4C4C4`,
            borderRadius: `20px`,
            fontSize:'20px',
            color:"black"
        } as CSSProperties)

        return { style }
    }
})
</script>

<style scoped>

</style>