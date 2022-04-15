<template >
  <div>
    <SidebarVue />
    <v-container>
      <v-row justify="center" class="mt-10">
        <v-col xl="6" lg="6" md="6" sm="8" xs="12">
          <nuxt-link to="/admin/category">
            <v-btn color="secondary" class="mb-4">Go Back</v-btn></nuxt-link
          >
          <v-card>
            <v-card-title> Update Category</v-card-title>
            <v-card-subtitle>
              <form action="" class="form">
                <v-text-field
                  label="Enter Category"
                  class="form__control"
                  hide-details="auto"
                >
                </v-text-field>

                <v-btn color="error" class="login__btn"> Update</v-btn>
              </form>
            </v-card-subtitle>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<script>
import SidebarVue from "../../../components/admin/Sidebar.vue";

export default {
  name: "EditCategoryPage",
   head(){
  return{
   title:'Update-Category',
  }
  },
  components: {
    SidebarVue,
  },
};
</script>
<style>
</style>