<template>
  <div class="card">
    <div class="card-header text-center" role="button">
      <strong>Montag</strong>
    </div>
    <div class="card-body">
      <div id="calendar-day">
        <!-- Anfang: Template für die Calendar-Event-Component -->
          <CalendarEvent />
        <!-- Ende: Template für die Calendar-Event-Component -->
      </div>
    </div>
  </div>
</template>
<script>
import CalendarEvent from "@/components/CalendarEvent.vue";
export default {
  name: "CalendarDay",
  components: {
    CalendarEvent,
  }
}
</script>
<style scoped >

</style>