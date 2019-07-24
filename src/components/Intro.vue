<template>
  <div>
    <div class="row">

      <div class="col-4">
        <div class="ab-portrait">
          <img src="BIO IMAGE" />
          <h1>Ash Blue</h1>
          <h2>Senior Web Developer</h2>
          <ul>
            <li><a target="_blank" href="#">GitHub</a></li>
            <li><a target="_blank" href="#">Twitter</a></li>
            <li><a target="_blank" href="https://www.linkedin.com/in/ashblue/">LinkedIn</a></li>
          </ul>
        </div>
      </div>

      <div class="col">
        <p>
          Hi, my name's <strong>Ash Blue</strong>. I'm a <em>senior web developer</em> leading teams
          to create web applications for 10+ years. My career has brought me everywhere from San
          Francisco's startup scene to fortune 500s. I specialize in JavaScript full stack with
          CI/CD to help empower teams to create cutting edge single page applications.
        </p>

        <h3>Details</h3>
        <ul>
          <li>Location: Denver</li>
          <li>Phone: 312-344-3792</li>
          <li>Email: ash@blueashes.com</li>
        </ul>

        <h2>Resume</h2>
        <button class="btn btn-primary">Resume PDF</button>
        <button class="btn btn-primary">Google Drive</button>
      </div>

    </div>

    <div class="footer">
      <p>This site is hosted and deployed through GitHub pages. Click here to see the source.</p>
      <p>Copyright</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Intro',
};
</script>

<style scoped>

</style>
