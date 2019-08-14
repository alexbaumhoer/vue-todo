<template>
  <li>
    <input type="checkbox" />
    {{ text }}
  </li>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class GroupListItem extends Vue {
  @Prop() text!: string;
}
</script>