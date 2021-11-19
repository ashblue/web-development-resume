<template>
  <div class="ab-resume">
    <h2 class="text-hide">My Resume</h2>

    <a
      target="_blank"
      href="https://www.dropbox.com/s/g4qs3w85qqldu1s/Resume-Ash-Blue.pdf?dl=0"
      class="btn btn-primary btn-lg btn-block mb-2">
      <Icon namespace="fas" icon="file-pdf" />&nbsp;
      View Resume
    </a>
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
