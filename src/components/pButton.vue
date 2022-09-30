<template>
    <div :style="active?{...style,...selectedStyle}:style">
        <slot></slot>
    </div>
</template>

<script lang="ts">
import { CSSProperties, defineComponent, ref } from 'vue'

export default defineComponent({
    props:{
        active:{
            type:Boolean,
            default:false
        }
    },
    setup() {
        const style = ref({
            width: `200px`,
            height: `74px`,
            left: `7537px`,
            top: `3791px`,
            background: `#F8F8F8`,
            boxShadow: `0px 4px 8px rgba(0, 0, 0, 0.02), 0px 2px 4px rgba(0, 0, 0, 0.02)`,
            borderRadius: `12px`,
            display: 'flex',
            justifyContent: 'center',
            alignItems: "center",
            fontSize: '24px',
        } as CSSProperties)
        const selectedStyle = ref({ backgroundColor: '#68BCF8',color:"white" } as CSSProperties)

        return { style,selectedStyle }
    }
})
</script>

