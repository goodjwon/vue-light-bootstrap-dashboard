<template>
  <div class="content">
    <div class="container-fluid">
      <div class="row">
        <div class="col-md-7">
          <edit-gallery-form>
          </edit-gallery-form>
        </div>
        <div class="col-md-5">
            <file-upload-form>
            </file-upload-form>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
    import EditGalleryForm from './Gallery/EditGalleryForm'
    import FileUploadForm from "./Gallery/FileUploadForm";
    export default {
        components: {
            EditGalleryForm,
            FileUploadForm
        }
    }

</script>
<style>

</style>
