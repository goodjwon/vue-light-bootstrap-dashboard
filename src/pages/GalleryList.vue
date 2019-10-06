<template>
  <div class="content">
    <div class="container-fluid">
      <div class="row">
        <gallery>
        </gallery>
      </div>
      <div class="row">
        <button type="submit" class="btn btn-info btn-fill float-left" @click.prevent="updateProfile">
          이미지 등록하기
        </button>
      </div>
    </div>
  </div>
</template>
<script>
  import gallery from './Gallery/Gallery.vue'

  export default {
    components: {
        gallery
    }
  }
</script>

