<template>
    <div style="position:relative">
        <div :style="style"></div>
      
        <img  src="../assets/curtainsleft.png">
        <img  src="../assets/curtainsright.png">
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
        return { style }
    }
})
</script>

<style scoped>

</style>