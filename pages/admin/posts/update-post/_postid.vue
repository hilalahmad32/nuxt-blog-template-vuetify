<template >
  <div>
    <SidebarVue />
    <v-container>
      <v-row justify="center" class="mt-10">
        <v-col xl="6" lg="6" md="6" sm="8" xs="12">
          <nuxt-link to="/admin/post">
            <v-btn color="secondary" class="mb-4">Go Back</v-btn></nuxt-link
          >
          <v-card>
            <v-card-title> Update Post</v-card-title>
            <v-card-subtitle>
              <form action="" class="form">
                <v-text-field
                  label="Enter Titile"
                  class="form__control"
                  hide-details="auto"
                  outlined
                >
                </v-text-field>
                <v-select class="mt-3" label="Standard" outlined></v-select>
                <v-textarea
                  class="form__control"
                  label="Enter description"
                  outlined
                ></v-textarea>
                <v-file-input
                  accept="image/*"
                  label="File input"
                  outlined
                ></v-file-input>

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
import SidebarVue from "~/components/admin/Sidebar.vue";

export default {
  name: "updatePostPage",
   head(){
  return{
   title:'Update-Post',
  }
  },
  components: {
    SidebarVue,
  },
};
</script>
<style>
</style>