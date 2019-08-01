<template>
    <div>
      <h3 class="text-hide">Details</h3>

      <ListDetails :detail-lines="details" />
    </div>
</template>

<script>
import ListDetails, { DetailLineData } from '../../molecules/ListDetails.vue';

function getBirthday() {
  const birthday = new Date(1987, 8, 25);
  const difference = Date.now() - birthday.getTime();
  return new Date(difference).getUTCFullYear() - 1970;
}

export default {
  name: 'DetailsComponent',
  components: {
    ListDetails,
  },
  data: () => ({
    details: [
      new DetailLineData('Age', 'clock', 'fas', getBirthday()),
      new DetailLineData('Location', 'map-marker', 'fas', 'Denver'),
      new DetailLineData('Phone', 'phone', 'fas', '<a href="tel:312-344-3792">312-344-3792</a>'),
      new DetailLineData('Email', 'envelope', 'fas', '<a href="mailto:ash@blueashes.com">ash@blueashes.com</a>'),
    ],
  }),
};
</script>
