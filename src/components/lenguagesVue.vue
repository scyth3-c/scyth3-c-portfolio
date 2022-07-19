<template>
  <b-container>
    <b-card variant="dark" class="shadow-lg rounded mt-5">
      <span class="text-dark font-weight-bold">percentage of use </span>
      <br />
      <span class="text-secondary"> (this does not represent the level) </span>
      <hr />
      <br />
      <div v-for="bar in bars" :key="bar.value" class="row mb-2">
        <div class="col-md-7">
          <b-badge class="text-white col-ms-1" variant="dark">{{
            bar.title
          }}</b-badge>
          <b-progress
            :value="bar.value"
            variant="secondary"
            striped
            animated="animated"
          ></b-progress>
        </div>
      </div>
      <br />
    </b-card>
  </b-container>
</template>
<script>
export default {
    name: 'lenguagesVue',
    data() {
        return {
            bars: [
                {title: "C++", value: 75, variant: "primary"},
                {title: "Vue", value: 60, variant: "success"},
                {title: "JavaScript", value:70, variant: "warning"},
                {title: "TypeScript", value: 70, variant: "primary"},
                {title: "PHP", value: 50, variant: "danger"},
                {title: ".NET Core", value: 56, variant: "primary"},
            ]
        }
    }
}
</script>
