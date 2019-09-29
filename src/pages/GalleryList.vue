<template>
  <div class="content">
    <div class="container-fluid">
      <div class="row">
        <div class="col-md-4">
          <gallery>
          </gallery>
        </div>
      </div>
      <div class="row">
        <div class="col-md-4">
          <button type="submit" class="btn btn-info btn-fill float-left" @click.prevent="updateProfile">
            이미지 등록하기
          </button>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
  import gallery from './UserProfile/Gallery.vue'

  export default {
    components: {
        gallery
    }
  }
</script>

