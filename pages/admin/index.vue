<template >
  <div class="margin__card">
    <v-row justify="center">
      <v-col xl="4" lg="4" md="6" sm="8" xs="12">
        <v-card>
          <v-card-title><h2>Admin Login</h2></v-card-title>
          <v-card-actions>
            <form action="" class="form">
              <v-text-field
                label="Enter Username"
                class="form__control"
                hide-details="auto"
              >
              </v-text-field>
              <v-text-field
                label="Enter Passwird"
                class="form__control"
                hide-details="auto"
              >
              </v-text-field>
              <v-btn color="error" class="login__btn"> Login</v-btn>
            </form>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>
<script>
export default {
  head(){
  return{
   title:'Login',
  }
  },
  comp
};
</script>
<style la>
</style>