<script>
import '../../../node_modules/@togakure/styles/lib/css/06-components/tooltip.css';

import { styles } from '@togakure/styles';
const classes = styles.tooltip;
export default {
  name: 'tog-tooltip',
  data: () => {
    return {
      classes
    };
  },
  props: {
    label: {
      type: String,
      required: true,
    },
    type: {
      type: String,
      default: 'default'
    }
  },
  computed: {
  }
};
</script>

<template>
  <div :class="[
    classes[type]
  ]">{{ label }}</div>
</template>
