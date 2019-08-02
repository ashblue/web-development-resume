<template>
  <div class="ab-resume">
    <h2 class="text-hide">My Resume</h2>

    <a
      target="_blank"
      href="https://docs.google.com/document/d/1gp4HYCqg0lmjAu0Kec9uRS9y_Z5gCf7UGIV7YKf0UIo/export?format=pdf&id=1gp4HYCqg0lmjAu0Kec9uRS9y_Z5gCf7UGIV7YKf0UIo&token=AC4w5ViGjzNzp-tkNg_qW9n_PJP415kNFQ%3A1366077437776"
      class="btn btn-primary btn-lg btn-block mb-2">
      <Icon namespace="fas" icon="file-pdf" />&nbsp;
      Download Resume
    </a>

    <p class="small text-muted text-center">
      Resume available in multiple formats via
      <a
        target="_blank"
        href="https://docs.google.com/document/d/1gp4HYCqg0lmjAu0Kec9uRS9y_Z5gCf7UGIV7YKf0UIo/edit?usp=sharing">Google Drive <Icon icon="google-drive" /></a>
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
