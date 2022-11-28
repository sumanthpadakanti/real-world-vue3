<template>
  <h1>Events for good</h1>
  <div class="events">
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
import EventCard from '@/components/EventCard.vue';

export default {
  name: 'HomeView',
  components: {
    EventCard,
  },
  data() {
    return {
      events: [
        {
          id: 100,
          category: 'Animal Welfare',
          title: 'Cat Adaoption Day',
          description: 'Find your new friend',
          location: 'Meow Town',
          date: '24th Nov 2022',
          time: '12.00 PM',
          petsAllowed: true,
        },
        {
          id: 101,
          category: 'Community',
          title: 'Community Gardening',
          description: 'Find your new friend',
          location: 'Meow Town',
          date: '25th Nov 2022',
          time: '12.00 PM',
          petsAllowed: true,
        },
        {
          id: 101,
          category: 'Watering',
          title: 'Watering plants',
          description: 'Find your new friend',
          location: 'Meow Town',
          date: '25th Nov 2022',
          time: '12.00 PM',
          petsAllowed: true,
        },
      ],
    };
  },
};
</script>
<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
