<template>
  <div>
    <h1>{{ title }}</h1>
    <ul>
      <GroupListItem text="List item" />
      <GroupListItem text="List item" />
      <GroupListItem text="List item" />
    </ul>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';
import GroupListItem from './GroupListItem.vue';

@Component({
  components: {
    GroupListItem,
  },
})
export default class Group extends Vue {
  @Prop() title!: string;
}
</script>