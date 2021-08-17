<template>
  <div class="profile">
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-lg-6">
          <div class="media text-left">
            <img src="../assets/user-pic.jpg" class="mr-3 user-pic" alt="..." />
            <div class="media-body">
              <h5 class="mt-0">Aldycky Bagus Witjaksana</h5>
              Cras sit amet nibh libero, in gravida nulla. Nulla vel metus
              scelerisque ante sollicitudin.
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

import "bootstrap/dist/css/bootstrap.css";

export default {
  name: "Profile",
  components: {},
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
