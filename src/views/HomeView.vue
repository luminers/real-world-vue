<template>
  <div class="events">
    <h1>Eventos</h1>
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from "@/components/EventCard.vue";

export default {
  name: "HomeView",
  components: {
    EventCard,
  },
  data() {
    return {
      events: [
        {
          id: 123456,
          category: "animal Welfare",
          title: "Cat adoption day",
          description: "Find your new feline friend.",
          location: "meow town",
          date: "june 5, 2022",
          time: "12:00",
          petsAllowed: true,
          organizer: "kat Laydee",
        },
        {
          id: 1253456,
          category: "animal Welfare",
          title: "Cat adoption day",
          description: "Find your new feline friend.",
          location: "meow town",
          date: "june 5, 2022",
          time: "12:00",
          petsAllowed: true,
          organizer: "kat Laydee",
        },
        {
          id: 1243456,
          category: "animal Welfare",
          title: "Cat adoption day",
          description: "Find your new feline friend.",
          location: "meow town",
          date: "june 5, 2022",
          time: "12:00",
          petsAllowed: true,
          organizer: "kat Laydee",
        },
      ],
    };
  },
};
</script>

<style scoped>
.events {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-flow: column wrap;
}
</style>
