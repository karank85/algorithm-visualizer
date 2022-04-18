<template>
  <v-app
    style="background-color: black"
    class="d-flex justify-center text-center"
  >
    <div>
      <v-row class="pt-5">
        <v-col cols="6" class="text-right">
          <v-btn color="primary" class="px-5">Binary Search</v-btn>
        </v-col>
        <v-col cols="6">
          <v-btn color="primary" class="px-5">Linear Search</v-btn>
        </v-col>
      </v-row>
      <v-row class="py-12 pl-5 justify-center">
        <v-card
          color="yellow"
          class="mx-2 px-5 py-5"
          :key="item.id"
          v-for="item in items"
        >
          {{ item }}
        </v-card>
        <v-card color="yellow" class="mx-2 px-5 py-5"> + </v-card>
      </v-row>
      <v-row class="py-12">
        <v-col cols="6" class="text-right">
          <v-btn color="primary" class="px-5">Clear</v-btn>
        </v-col>
        <v-col cols="6">
          <v-btn color="primary" class="px-5">Generate Random</v-btn>
        </v-col>
      </v-row>
    </div>
  </v-app>
</template>

<script>
export default {
  name: "HomePage",
  data() {
    return {
      items: [1, 2, 3],
    };
  },
};
</script>

<style scoped></style>
