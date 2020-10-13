<template>
    <div>
        <div class="absolute -my-10">
            <schedule-toggle :value="schedule"></schedule-toggle>
        </div>
        <plan-card name='Starter' monthly='19' :selected="true" :features="[
            '5,000 downloads / month',
            'Unlimited shows and episodes',
            'Analytics, teams, and more...',
        ]"></plan-card>
        <plan-card name='Professional' monthly='49' :selected="false" :features="[
            '15,000 downloads / month',
            'Unlimited shows and episodes',
            'Analytics, teams, and more...',
        ]"></plan-card>
        <plan-card name='Small Business' monthly='99' :selected="false" :features="[
            '45,000 downloads / month',
            'Unlimited shows and episodes',
            'Analytics, teams, and more...',
        ]"></plan-card>
    </div>
</template>

<script>
import PlanCard from './PlanCard'
import ScheduleToggle from './ScheduleToggle'

export default {
  name: 'App',
  components: {
      PlanCard,
      ScheduleToggle,
  },
  props: [],
  data() {
      return {
          schedule: 'monthly',
      }
  },
  methods: {

  },
}
</script>

<style>

</style>