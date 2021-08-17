<template>
  <div class="container mt-5">
    <div class="row header p-3">
      <div class="col-lg-12">
        <h2>What I do today?</h2>
      </div>
    </div>
    <div class="row content mt-3">
      <div class="col-lg-12">
        <div class="pekerjaan-rumah">
          <div class="row">
            <div
              v-for="tugasSaya in tugas"
              v-bind:key="tugasSaya.id"
              class="col-lg-12 mb-2 text-left tugas"
            >
              <div class="form-check">
                <input
                  class="form-check-input"
                  onclick=""
                  type="checkbox"
                  value=""
                  id="defaultCheck1"
                />
                <label
                  class="form-check-label item"
                  v-bind:class="{ 'item-completed': tugasSaya.isDone }"
                  for="defaultCheck1"
                >
                  {{ tugasSaya.deskripsi }}
                </label>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Tugas",
  data: function() {
    return {
      tugas: [
        {
          id: 1,
          deskripsi: "Mengerjakan tugas proyek kuliah",
          isDone: false,
        },
        {
          id: 2,
          deskripsi: "Melanjutkan pembuatan project website",
          isDone: false,
        },
        {
          id: 3,
          deskripsi: "Menonton film dan youtube",
          isDone: false,
        },
        {
          id: 4,
          deskripsi: "Main game",
          isDone: false,
        },
      ],
    };
  },
  components: {},
};
</script>

<style scoped>
.header {
  background: #1abc9c;
}

.header h2 {
  margin: 0;
}

.tugas .item {
  font-size: 18px;
}

.item-completed {
  color: #1abc9c;
}
</style>
