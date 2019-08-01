<template>
  <div>
    <div class="row mt-4 mb-5">
      <div class="col-4 d-none d-lg-block">
        <BioCard />
      </div>

      <div class="col">
        <h2 class="text-lowercase h1">
          About Me
        </h2>

        <p>
          Hi, I'm <strong>Ash Blue</strong>. A <em>senior web developer</em> with 10+
          years of experience creating web applications. My career has brought me from
          San Francisco's startup scene to fortune 500s. I specialize in JavaScript full stack with
          CI/CD to help teams create cutting edge solutions.
        </p>

        <DetailsCollection class="mb-5" />

        <Resume />
      </div>
    </div>
  </div>
</template>

<script>
import BioCard from '../bio-cards/BioCard.vue';
import Resume from './Resume.vue';
import DetailsCollection from './DetailsCollection.vue';

function getBirthday() {
  const birthday = new Date(1987, 8, 25);
  const difference = Date.now() - birthday.getTime();
  return new Date(difference).getUTCFullYear() - 1970;
}

export default {
  name: 'Intro',
  components: {
    Resume,
    DetailsCollection,
    BioCard,
  },
  data: () => ({
    age: getBirthday(),
  }),
};
</script>
