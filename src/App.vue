<template>
  <div>
    <p-button>washroom</p-button>
    <p-button :active="true">childroom</p-button>
    <c-button>close</c-button>
    <c-button>open</c-button>
    <c-button>
      <img src='./assets/Polygon.png'>
    </c-button>
    <p-switch></p-switch>
    <p-slider></p-slider>
    <p-select></p-select>
    <lamp></lamp>
    <lock></lock>
    <Camera></Camera>
    <roller-shutter></roller-shutter>
    <curtains></curtains>
    <color-temperature></color-temperature>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import CButton from './components/cButton.vue'
import Lamp from './components/lamp.vue'
import Lock from './components/lock.vue'
import pButton from './components/pButton.vue'
import PSelect from './components/pSelect.vue'
import PSlider from './components/pSlider.vue'
import pSwitch from './components/pSwitch.vue'
import Camera from './components/camera/index.vue'
import RollerShutter from './components/rollerShutter.vue'
import Curtains from './components/curtains.vue'
import ColorTemperature from './components/colorTemperature.vue'

export default defineComponent({
  components: { pButton, CButton, pSwitch, PSlider, PSelect, Lamp, Lock, Camera, RollerShutter, Curtains, ColorTemperature },
  setup() {


    return {}
  }
})
</script>

<style scoped>

</style>