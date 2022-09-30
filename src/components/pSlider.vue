<template>
    <div :style="style">
        <div :style="buttonStyle"></div>
    </div>
</template>

<script lang="ts">
import { CSSProperties, defineComponent, ref } from 'vue'

export default defineComponent({
    setup() {
        const style = ref({
            width: `100%`,
            height: `2px`,
            background: `linear-gradient(270deg, #CCD1FF 6.2%, #4D74FE 90.96%)`,
            position: "relative"
        } as CSSProperties)
        const buttonStyle = ref({
            width: "24px",
            height: "24px",
            backgroundColor: "#6887FD",
            borderRadius: "50%",
            position: "absolute",
            top: "-11px",
            border: `2px solid #FFFFFF`,
            boxShadow: `0px 4px 8px rgba(0, 0, 0, 0.04), 0px 2px 4px rgba(0, 0, 0, 0.04), inset 0px -2px 0px rgba(223, 223, 223, 0.25)`,

        } as CSSProperties)


        return { style, buttonStyle }
    }
})
</script>

<style scoped>

</style>