<template>
  <card>
    <h4 slot="header" class="card-title">Edit Gallery</h4>
    <form>
      <h5>User Profile</h5>
      <div class="row">
        <div class="col-md-5">
          <base-input type="text"
                      label="Writer(작성자)"
                      :disabled="true"
                      placeholder="제목을 입력 하세요.."
                      v-model="posts.writer">
          </base-input>
        </div>
        <div class="col-md-3">
          <base-input type="text"
                      label="User Id"
                      :disabled="true"
                      placeholder="Username"
                      v-model="posts.userid">
          </base-input>
        </div>
        <div class="col-md-4">
          <base-input type="email"
                      label="User Email"
                      placeholder="Email"
                      v-model="posts.email">
          </base-input>
        </div>
      </div>

      <h5>Category Info</h5>
      <div class="row">
        <div class="col-md-6">
          <base-input type="text"
                      label="Category Name "
                      :disabled="true"
                      placeholder="First Name"
                      v-model="posts.postGroupName">
          </base-input>
        </div>
        <div class="col-md-6">
          <base-input type="text"
                      label="Category Code"
                      :disabled="true"
                      placeholder="Last Name"
                      v-model="posts.postGroupKey">
          </base-input>
        </div>
      </div>

      <div class="row">
        <div class="col-md-12">
          <base-input type="text"
                      label="Title"
                      placeholder="Home Address"
                      v-model="posts.title">
          </base-input>
        </div>
      </div>

      <div class="row">
        <div class="col-md-12">
          <base-input label="Contents">
            <textarea class="form-control" id="exampleFormControlTextarea3" rows="3" v-model="posts.body"></textarea>
          </base-input>
        </div>
      </div>

      <div class="text-center">
        <button type="submit" class="btn btn-info btn-fill float-right" @click.prevent="updateProfile">
          Update Profile
        </button>
      </div>
      <div class="clearfix"></div>
    </form>
  </card>
</template>

<script>
    import Card from 'src/components/Cards/Card.vue'

    export default {
        components: {
            Card
        },
        data () {
            return {
                posts: {
                    title: '혼례장 소개...',
                    body: 'post 답글 입력 테스트 post 내용 입력 테스트 중3' +
                        '\r\npost 답글 입력 테스트 post 내용 입력 테스트 중3' +
                        '\r\npost 답글 입력 테스트 post 내용 입력 테스트 중3',
                    writer: '우리옛멋ㅇㅇㅇ',
                    userid: 'gonji500',
                    groupNum: '156729890939283',
                    postKey: '156729894619269',
                    modDate: null,
                    regDate: '2019-09-01 00:49:06.192',
                    depth: '1',
                    postGroupKey: '128763846762687',
                    postGroupName: '장소소개',
                    files: []
                }
            }
        },
        methods: {
            updateProfile () {
                alert('Your data: ' + JSON.stringify(this.posts))
            }
        }
    }

</script>

<style scoped>

</style>
