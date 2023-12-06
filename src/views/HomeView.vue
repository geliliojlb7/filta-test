<script>
import Banner from '../components/Banner.vue'
import CardSection from '../components/CardSection.vue'

export default {
  components: {
    Banner,
    CardSection,
  },
  data() {
    return {
      cards: [
        {
          title: "Card 1",
          description: "Lorem ipsum dolor sit amet, consectetur adipiscing, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua, Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.",
        },
        {
          title: "Card 2",
          description: "Lorem ipsum dolor sit amet, consectetur adipiscing, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
        },
        {
          title: "Card 3",
          description: "Lorem ipsum dolor sit amet, consectetur adipiscing, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua, Ut enim ad minim veniam, quis nostrud exercitation ullamco.",
        },
      ],
    };
  },
};
</script>

<template>
  <Banner title="Hello Developer!" details="Lorem ipsum dolor sit amet, consectetur adipiscing elit"/>
  <CardSection :cards="cards" />
</template>