<template functional>
  <span :aria-hidden="props.decorative" :aria-label="props.title" class="pencil-icon" role="img" v-on="listeners">
    <svg :fill="props.fillColor" class="icon__svg" :width="props.size" :height="props.size" viewBox="0 0 24 24">
      <path
        d="M11 3a1 1 0 01.117 1.993L11 5H4a1 1 0 00-.993.883L3 6v14a1 1 0 00.883.993L4 21h14a1 1 0 00.993-.883L19 20v-7a1 1 0 011.993-.117L21 13v7a3 3 0 01-2.824 2.995L18 23H4a3 3 0 01-2.995-2.824L1 20V6a3 3 0 012.824-2.995L4 3h7zm6.793-1.207a3.121 3.121 0 014.414 4.414l-9.5 9.5a1 1 0 01-.464.263l-4 1a1 1 0 01-1.213-1.213l1-4a1 1 0 01.263-.464zm3 1.414a1.121 1.121 0 00-1.586 0l-9.304 9.304-.529 2.114 2.114-.529 9.305-9.303a1.122 1.122 0 00.087-1.488z"
        fill-rule="evenodd"
      ></path>
    </svg>
  </span>
</template>

<script>
export default {
  name: 'Pencilicon',
  props: {
    title: {
      type: String,
      default: 'Pencil icon',
    },
    decorative: {
      type: Boolean,
      default: false,
    },
    fillColor: {
      type: String,
      default: 'currentColor',
    },
    size: {
      type: Number,
      default: 24,
    },
    viewBox: {
      type: String,
      default: '0 0 24 24',
    },
  },
};
</script>
