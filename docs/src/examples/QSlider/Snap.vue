<template>
  <div class="q-pa-md">
    <q-chip square color="secondary" text-color="white">
      Model: {{ value }} (-20 to 20)
    </q-chip>
    <q-slider
      v-model="value"
      :min="-20"
      :max="20"
      :step="4"
      label
      label-always
      color="purple"
    />
  </div>
</template>

<script>
export default {
  data () {
    return {
      value: 0
    }
  }
}
</script>
