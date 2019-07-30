<template>
  <div>
    <div class="row mt-5">
      <div class="col-12 col-lg-4">
        <BioCard class="mb-sm-4" />
      </div>

      <div class="col">
        <p>
          Hi, my name's <strong>Ash Blue</strong>. I'm a <em>senior web developer</em> with 10+
          years of experience creating web applications. My career has brought me everywhere from
          San Francisco's startup scene to fortune 500s. I specialize in JavaScript full stack with
          CI/CD to help empower teams to create cutting edge solutions.
        </p>

        <h3>Details</h3>
        <ul>
          <li>Location: Denver</li>
          <li>Phone: 312-344-3792</li>
          <li>Email: ash@blueashes.com</li>
        </ul>

        <h2>Resume</h2>
        <button class="btn btn-primary">Resume PDF</button>
        <button class="btn btn-primary">Resume Word</button>
        <button class="btn btn-primary">Resume Google Drive</button>
      </div>
    </div>

    <div class="footer">
      <p>This site is hosted and deployed through GitHub pages. Click here to see the source.</p>
      <p>Copyright</p>
    </div>
  </div>
</template>

<script>
import BioCard from './BioCard.vue';

export default {
  name: 'Intro',
  components: { BioCard },
};
</script>

<style scoped>

</style>
