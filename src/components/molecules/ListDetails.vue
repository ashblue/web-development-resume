<template>
  <div>
    <DetailLine
      v-for="detail in detailLines"
      :key="detail.title"
      :title="detail.title"
      :icon="detail.icon"
      :icon-namespace="detail.iconNamespace">
      <span v-html="detail.text"></span>
    </DetailLine>
  </div>
</template>

<script>
import DetailLine from '../atoms/DetailLine.vue';

export class DetailLineData {
  constructor(title, icon, iconNamespace, text) {
    this.title = title;
    this.icon = icon;
    this.iconNamespace = iconNamespace;
    this.text = text;
  }
}

export default {
  name: 'ListDetails',
  components: {
    DetailLine,
  },
  props: {
    detailLines: Array,
  },
};
</script>
