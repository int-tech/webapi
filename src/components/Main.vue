<template>
  <div class="main">
    <!-- <form v&#45;on:submit.prevent="onSubmit"> -->

        <!-- file upload -->
        <label>1. What file do you want to upload?</label>
        <div class="main_file">
          <input type="file" id="image" name="file" ref="file" v-on:change="handleFileUpload()" />
        </div>

        <!-- raido buttons -->
        <label>2. Which one is written?</label>
        <div class="main_radio ui form">
          <!-- number -->
          <div class="inline fields">
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency" checked="checked" v-model="picked" value='0'><label>0</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='1'><label>1</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='2'><label>2</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='3'><label>3</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='4'><label>4</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='5'><label>5</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='6'><label>6</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='7'><label>7</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='8'><label>8</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='9'><label>9</label>
            </div></div>
          </div>

          <!-- alphabet -->
          <div class="inline fields">
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='a'><label>a</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='b'><label>b</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='c'><label>c</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='d'><label>d</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='e'><label>e</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='f'><label>f</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='g'><label>g</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='h'><label>h</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='i'><label>i</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='j'><label>j</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='k'><label>k</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='l'><label>l</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='m'><label>m</label>
            </div></div>
          </div>
          <div class="inline fields">
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='n'><label>n</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='o'><label>o</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='p'><label>p</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='q'><label>q</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='r'><label>r</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='s'><label>s</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='t'><label>t</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='u'><label>u</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='v'><label>v</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='w'><label>w</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='x'><label>x</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='y'><label>y</label>
            </div></div>
            <div class="field"><div class="ui radio checkbox">
              <input type="radio" name="frequency"  v-model="picked" value='z'><label>z</label>
            </div></div>
          </div>
        </div>

      <button class="positive ui button" v-on:click="submitFile()">Submit</button>
    <!-- </form> -->

    <div class="response_image">
      <!-- <img id="imgTest" src="../assets/logo.png"> -->
      <img id="imgTest"/>
    </div>

  </div>
</template>

<script>
// const ENDPOINT = 'http://127.0.0.1:3000';
const ENDPOINT = 'http://54.201.208.182:3000';
const axios = require('axios')
export default {
  name: 'Main',
  data() {
    return {
      picked: '',
      file: ''
    }
  },
  methods: {
    handleFileUpload() {
      // set a local variable to the value of the file uploaded
      console.log(this.picked)
      this.file = this.$refs.file.files[0]
    },
    async getFile(file_name) {
      let res_get = await axios.get(`${ENDPOINT}/${file_name}`, {
        responseType: 'blob'
      });

      if ( res_get.status === 200) {
        var reader = new FileReader();
        reader.onloadend = function() {
          var img = document.getElementById("imgTest");
          img.src = reader.result;
        }
        // DataURLとして読み込む
        reader.readAsDataURL(res_get.data);
      } else {
        alert('false')
      }
    },
    async submitFile() {
      try {
        let formData = new FormData()
        if (this.file !== '') {
          formData.append('file', this.file)
          formData.append('picked', this.picked)
        }

        let res = await axios.post(`${ENDPOINT}/image`, formData,{
          headers: {
            'Content-Type': 'multipart/form-data'
          }
        })

        if (res.status !== 200) {
          alert('failed!')
        }

        this.getFile(this.file.name)

        // let res_get = await axios.get(`${ENDPOINT}/${this.file.name}`, {
        //   responseType: 'blob'
        // });
        //
        // if ( res_get.status === 200) {
        //   var reader = new FileReader();
        //   reader.onloadend = function() {
        //     var img = document.getElementById("imgTest");
        //     img.src = reader.result;
        //   }
        //   // DataURLとして読み込む
        //   reader.readAsDataURL(res_get.data);
        // } else {
        //   alert('false')
        // }

      // let res = await axios.get(`${ENDPOINT}/${this.file.name}`, {
      //   responseType: 'blob'
      // })
      // let res = await axios.get(`${ENDPOINT}/${this.file.name}`)

      // if (res.status !== 200) {
      //   throw new Error('response error: failed to get image')
      // }

      // var img = document.getElementById("imgTest");
      // var url = window.URL || window.webkitURL;
      // // document.querySelector("#imgTest").src = url.createObjectURL(res.data)
      // const blob_url = url.createObjectURL(res.data)
      // console.log(blob_url)
      // alert(blob_url)
      } catch (e) {
        throw new Exception(e)
      }
    }
  }
}
</script>

<style>
  .main{
    width:50%;
    margin: 50px auto;
    text-align:left;
  }
  .main_file{
    width: 50%;
    margin: 30px 0px;
    text-align:left;
  }
  .main_radio{
    width: 50%;
    margin: 30px 0px;
  }
  .response_image{
    width:400px;
    height:400px;
  }
  .response_image img{
    width:100%;
    height:100%;
  }
</style>
