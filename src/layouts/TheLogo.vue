<template>
  <svg
    id="Calque_1"
    class="the-logo"
    data-name="Calque 1"
    xmlns="http://www.w3.org/2000/svg"
    viewBox="0 0 229.7 220.62"
  >
    <g>
      <path
        class="cls-1"
        d="m106.14,18.29v38.36s.43,11.53-12.2,11.53-11.97-9.53-11.97-9.53v-15.63c0-3.34-3.62-5.41-6.52-3.74-30.47,17.55-38.49,42.32-40.58,52.94-.53,2.68,1.52,5.16,4.25,5.16h53.54s60.27.15,60.27.15"
      />
      <path
        class="cls-1"
        d="m88.83,8.09S9.01,21.84,9.01,110.08s79.82,103.33,79.82,103.33c4.14,1.03,17.29,1.18,17.29-11.23v-40.21s.44-10.2-12.27-10.2-11.97,10.35-11.97,10.35v15.75c0,3.31-3.55,5.38-6.44,3.78-10.89-6.03-32.54-21.74-40.57-54.29-.68-2.75,1.43-5.41,4.26-5.38l53.64.7,65.46-.8"
      />
      <path class="cls-1" d="m106.14,21.17c-.23-1.03,2.22-18.25-18.83-12.77" />
    </g>
    <path
      class="cls-1"
      d="m156.74,121.91l15.14-.14h18.03c2.72,0,4.78,2.48,4.25,5.15-2.16,10.96-10.4,36.94-41,53.7-2.9,1.59-6.44-.48-6.44-3.78v-54.99"
    />
    <path
      class="cls-1"
      d="m123.07,97.03V14.25c0-9.73,12.12-7.16,12.12-7.16,3.33-.21,8.35.79,11.53,1.66,26.16,7.17,53.61,30.05,60.43,43.97,1.7,3.47,2.49,7.12.99,10.53-1.73,3.97-4.64,5.95-7.83,6.94-5.87,1.83-12.25-.17-16.44-4.67-2.3-2.47-3.67-4.93-5.64-8.25-6.46-10.92-13.14-16.37-20.92-19.86-2.02-.9-4.34-1.03-6.38-.19-2.11.86-4.21,2.72-4.21,6.71v53.57"
    />
    <path class="cls-1" d="m171.88,97.52s-14.21,0-19.75,0" />
    <path
      class="cls-1"
      d="m171.88,97.52s22.44,0,35.44.59c13.01.59,13.3,12.41,13.3,12.41,0,0,2.07,27.5-17.44,57.36-19.51,29.86-44.94,38.73-60.31,44.05-7.69,2.66-12.64.37-15.67-2.59-2.74-2.67-4.14-6.42-4.14-10.24v-76.89"
    />
  </svg>
</template>

<script setup lang="ts">
import { computed } from 'vue';

interface Props {
  size?: string;
}

const props = withDefaults(defineProps<Props>(), {
  size: '40px',
});

const sizeLogo = computed<string>(() => {
  return props.size;
});
</script>

<style lang="scss">
.the-logo {
  height: v-bind(sizeLogo);
  width: v-bind(sizeLogo);

  .cls-1 {
    fill: none;
    stroke: var(--q-primary);
    stroke-miterlimit: 10;
    stroke-width: 8px;
  }
}
</style>
