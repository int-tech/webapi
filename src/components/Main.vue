<template>
  <div class="main">
    <form>
      <input type="file" id="image" name="file" ref="file" v-on:change="handleFileUpload()" />
      <button class="positive ui button" v-on:click="submitFile()">Submit</button>
    </form>
  </div>
</template>

<script>
const axios = require('axios')
export default {
  name: 'Main',
  datq() {
    return {
      file: ''
    }
  },
  methods: {
    handleFileUpload() {
      // set a local variable to the value of the file uploaded
      this.file = this.$refs.file.files[0]
    },
    submitFile() {
      let formData = new FormData()
      if (this.file !== '') {
        formData.append('file', this.file)
      }
      
      axios.post('http://54.201.208.182:3000/image', formData,{
          headers: {
            'Content-Type': 'multipart/form-data'
          }
      })
      .then(function(res) {
        console.log(res)
      })
      .catch(function() {
        console.log('failed')
      })

    }
  }
}
</script>

<style>
  .main{
    margin: 50px
  }
</style>
