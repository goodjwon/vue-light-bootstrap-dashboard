<template>
  <card>
    <h4 slot="header" class="card-title">File Upload</h4>
    <form>
      <h5>User Profile</h5>

      <div class="row">
        <div class="col-md-12">
          <file-input @change="filesChange"></file-input>
          <b-form-file multiple :file-name-formatter="formatNames"></b-form-file>
          <div class="custom-file">
            <input type="file" class="custom-file-input" id="validatedCustomFile" required>
            <label class="custom-file-label" for="validatedCustomFile">Choose file...</label>
            <div class="invalid-feedback">Example invalid custom file feedback</div>
          </div>
        </div>
      </div>

      <div class="row">
        <div class="col-md-12">
          <div class="text-center">
            <button class="btn btn-primary btn-xs btn-fill float-left">Upload S3</button>
          </div>
        </div>
      </div>

      <div class="row">
        <div class="col-md-12">
          <card class="card-image">
            <img class="img-fluid"
                 src="https://ununsplash.imgix.net/photo-1431578500526-4d9613015464?fit=crop&fm=jpg&h=300&q=75&w=400"
                 alt="..."/>
          </card>
          <card class="card-image">
            <img class="img-fluid"
                 src="https://ununsplash.imgix.net/photo-1431578500526-4d9613015464?fit=crop&fm=jpg&h=300&q=75&w=400"
                 alt="..."/>
          </card>
        </div>
      </div>
    </form>
  </card>
</template>

<script>
    import Card from 'src/components/Cards/Card.vue'

    export default {
        components: {
            Card
        },
        data() {
            return {
                files: []
            }
        },
        methods: {
            filesChange(files) {
                this.files = files
            }
        }
    }


</script>

<style scoped>

</style>
