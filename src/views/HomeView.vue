<template>
  <div class="home">
    <div class="row">
      <div class="card col-6">
        <h1 align=" center">
         Inventory System
        </h1>

        <p class="card-text">

        </p>
      </div>

      <div class="card col-6">
        <apexchart width="580" type="donut" :options="options" :series="series"></apexchart>
      </div>
    </div>

    <div class="row">

      <div class="card col-3">
        <div class="ratio ratio-1x1">
          <img class="img-fluid img-thumbnail" style="object-fit:cover"
            src="https://cdn.elearningindustry.com/wp-content/uploads/2016/05/top-10-books-every-college-student-read-1024x640.jpeg"
            onclick="location.href = '/book'">
        </div>
        <p class="card-text">
          Books
        </p>
      </div>

      <div class="card col-3">
        <div class="ratio ratio-1x1">
          <img class="img-fluid img-thumbnail" style="object-fit:cover"
            src="https://hips.hearstapps.com/hmg-prod.s3.amazonaws.com/images/most-popular-video-games-of-2022-1642612227.png"
            onclick="location.href = '/game'">
        </div>
        <p class="card-text">
          Game
        </p>
      </div>

      <div class="card col-3">
        <div class="ratio ratio-1x1">
          <img class="img-fluid img-thumbnail" style="object-fit:cover"
            src="https://fuseinsurance.ca/wp-content/uploads/2020/12/joshua-lam-I2f_r0jj73U-unsplash-scaled-e1607536552512-1200x600.jpg"
            onclick="location.href = '/gifts'">
        </div>
        <p class="card-text">
          Gifts
        </p>
      </div>

      <div class="card col-3">
        <div class="ratio ratio-1x1">
          <img class="img-fluid img-thumbnail" style="object-fit:cover"
            src="https://www.structuralguide.com/wp-content/uploads/2022/01/Construction-Materials.jpg"
            onclick="location.href = '/materials'">
        </div>
        <p class="card-text">
          Materials
        </p>
      </div>
    </div>
  </div>


</template>

<script>
// @ is an alias to /src
//import HelloWorld from '@/components/HelloWorld.vue'
import { ref, onMounted } from "vue";
export default {
  name: 'HomeView',
  components: {
    //HelloWorld
  },


  setup() {
    const options = ref({});
    const series = ref([44, 55, 41, 17, 15]);

    onMounted(async () => {

      var response = await fetch("/api/bookings/aggregate/groupby");

      if (response.ok) {
        var heroes = await response.json();

        series.value = heroes.map(a => a.count);
        options.value = { labels: heroes.map(a => a._id) };
      }
    });
    return {
      options, series
    }
  }
}

</script>
