<template>
  <div class="event-card">
    <span>@ {{ event.time }} on {{ event.date }}</span>
    <h4>{{ event.title }}</h4>
  </div>
</template>

<script>
export default {
  name: "EventCard",
  props: {
    event: Object,
  },
};
</script>
<style scoped>
.event-card {
  margin: 10px;
  width: 400px;
  padding: 20px;
  border: 1px solid #000;
}
.event-card:hover {
  box-shadow: 10px 15px 40px #777;
}
</style>
