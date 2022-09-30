<template>
    <div :style="style">
        <div>
            <div><img src="../../assets/snap.png"></div>
            <div>snap</div>
        </div>
        <div>
            <div><img src="../../assets/video.png"></div>
            <div>video</div>
        </div>
        <div>
            <div><img src="../../assets/talk.png"></div>
            <div>talk</div>
        </div>
        <div>
            <div><img src="../../assets/hear.png"></div>
            <div>hear</div>
        </div>
    </div>
</template>

<script lang="ts">
import { CSSProperties, defineComponent, ref } from 'vue'

export default defineComponent({
    setup() {
        const style = ref({
            width: '100%',
            height: "148px",
            backgroundColor: "rgba(0,0,0,0.4)",
            borderRadius: "20px",
            display:"flex",
            justifyContent:"space-around",
            alignItems:"center",
            color:"white"
        } as CSSProperties)

        return { style }
    }
})
</script>

<style scoped>
.wewq{
    justify-content: space-around;
}
</style>