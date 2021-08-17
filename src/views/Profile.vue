<template>
  <div class="profile">
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-lg-6">
          <div class="media text-left">
            <img src="../assets/user-pic.jpg" class="mr-3 user-pic" alt="..." />
            <div class="media-body">
              <h5 class="mt-0">{{ firstName }} {{ lastName }}</h5>
              {{ bio }}
            </div>
          </div>
        </div>
      </div>
    </div>
    <Tugas />
  </div>
</template>

<script>
// @ is an alias to /src

import "bootstrap/dist/css/bootstrap.css";
import Tugas from "../components/Tugas.vue";

export default {
  name: "Profile",
  data: function() {
    return {
      firstName: "Aldycky",
      lastName: "Bagus",
      bio:
        "Hello!! Cras sit amet nibh libero, in gravida nulla. Nulla vel metus scelerisque ante sollicitudin.",
    };
  },
  components: {
    Tugas,
  },
};
</script>

<style scoped>
.user-pic {
  border-radius: 50%;
  height: 80px;
  width: 80px;
  object-fit: cover;
}
</style>
