<template>
  <div class="ab-resume">
    <h2 class="text-hide">My Resume</h2>

    <button class="btn btn-primary btn-lg btn-block mb-1">
      <Icon namespace="fas" icon="file-pdf" />&nbsp;
      Download Resume
    </button>

    <p class="small text-muted text-center">
      Resume available in multiple formats via
      <a href="#">Google Drive <Icon icon="google-drive" /></a>
    </p>
  </div>
</template>

<script>
import Icon from '../../atoms/Icon.vue';

export default {
  name: 'Resume',
  components: {
    Icon,
  },
};
</script>
