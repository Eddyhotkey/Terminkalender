<template>
  <div id="calender-week">
    <div class="card-group">
      <!-- Anfang: Template für die Calendar-Day-Component -->
      <CalendarDay v-for="i in 7 " :key="i" />
      <!-- Ende: Template für die Calendar-Day-Component -->
    </div>
  </div>
</template>

<script>
import CalendarDay from "@/components/CalendarDay.vue";
import Store from "../store";
export default {
  name: "CalendarWeek",


  data() {
    return {
      calendarWeekData: Store.state.calendarWeekData,
    };
  },

  components: {
    CalendarDay,
  }
};

</script>
<style scoped >

</style>