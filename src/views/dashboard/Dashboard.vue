<script setup lang="ts">
import { ref } from "vue";

// import TheSalesOverview from "./dashboardComponents/sales-overview/TheSalesOverview.vue";
// import DailyActivities from "./dashboardComponents/daily-activities/DailyActivities.vue";
// import ProductMonthTable from "./dashboardComponents/project-month-table/ProductMonthTable.vue";
import ButtonsDefault from "@/components/vuetifyComponents/buttons/ButtonsDefault.vue";
import BlogCard from "./dashboardComponents/blog-card/BlogCard.vue";

function download () {
  console.log('download');
}

function report () {
  console.log('report');
}

function upload () {
  console.log('upload');
}
</script>

<template>
  
  <v-row>
    <!-- <v-col cols="12" sm="12">
      <TheSalesOverview />
    </v-col>
    <v-col cols="12" lg="4" class="d-flex align-items-stretch">
      <DailyActivities />
    </v-col>
    <v-col cols="12" lg="8" class="d-flex align-items-stretch">
      <ProductMonthTable />
    </v-col>
    <v-col cols="12" sm="12">
    <BlogCard />
    </v-col> -->
    <div class="d-flex flex-wrap gap-2">
      <div>
        <v-btn color="secondary" @click="download">Download</v-btn>
      </div>
      <div>
        <v-btn color="secondary" @click="report">Report</v-btn>
      </div>
      <div>
        <v-btn color="secondary" @click="upload">Upload</v-btn>
      </div>
    </div>
  </v-row>
</template>
