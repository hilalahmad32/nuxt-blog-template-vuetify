<template>
  <div>
    <SidebarVue />
    <v-container>
      <v-card>
        <v-card-text class="d-flex justify-space-between align-center">
          <v-card-title> Post ( 33 ) </v-card-title>
          <v-card-actions>
            <nuxt-link to="/admin/posts/create-post">
              <v-btn color="red lighten-2"> New </v-btn>
            </nuxt-link>
          </v-card-actions>
        </v-card-text>
        <hr />

        <v-card-subtitle>
          <v-simple-table>
            <template v-slot:default>
              <thead>
                <tr>
                  <th class="text-enter">Id</th>
                  <th class="text-enter">Title</th>
                  <th class="text-enter">Category</th>
                  <th class="text-enter">image</th>
                  <th class="text-enter">Views</th>
                  <th class="text-enter">View</th>
                  <th class="text-enter">Edit</th>
                  <th class="text-enter">Delete</th>
                </tr>
              </thead>
              <tbody>
                <tr v-for="(item, index) in 5" :key="index">
                  <td class="">{{ index + 1 }}</td>
                  <td class="">category {{ index + 1 }}</td>
                  <td class="">Php</td>
                  <td class="">
                    <v-img
                      src="https://cdn.vuetifyjs.com/images/parallax/material.jpg"
                      width="70"
                      cover
                    ></v-img>
                  </td>
                  <td class="">44</td>
                  <td class="">
                    <v-btn
                      text
                      class="ma-2"
                      @click="view_dialog = true"
                      variant="text"
                      color="blue"
                    >
                      <v-icon color="green darken-3"> mdi-eye</v-icon>
                    </v-btn>
                  </td>
                  <td class="">
                    <nuxt-link to="/admin/posts/update-post/2">
                      <v-btn text class="ma-2" variant="text" color="blue">
                        <v-icon color="blue darken-3"> mdi-pencil</v-icon>
                      </v-btn></nuxt-link
                    >
                  </td>
                  <td class="">
                    <v-btn text class="ma-2" variant="text" color="red">
                      <v-icon color="red darken-3"> mdi-delete</v-icon>
                    </v-btn>
                  </td>
                </tr>
              </tbody>
            </template>
          </v-simple-table>
        </v-card-subtitle>
      </v-card>
    </v-container>
  </div>
</template>
<script>
import SidebarVue from "../../components/admin/Sidebar.vue";

export default {
  name: "PostPage",
  head(){
  return{
   title:'Post',
  }
  },
  components: {
    SidebarVue,
  },
};
</script>
<style>
</style>