<template>
    <div>
        <control></control>
        <navigation></navigation>
        <select-item></select-item>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import Control from './control.vue'
import Navigation from './navigation.vue'
import selectItem from './selectItem.vue'

export default defineComponent({
  components: { selectItem, Control, Navigation },
    setup () {
        

        return {}
    }
})
</script>

<style scoped>

</style>