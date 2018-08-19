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

    <div class="main_all_response_image">
      <div class="response_image">
        <img id="imgTest_0"/>
      </div>
      <div class="response_image">
        <img id="imgTest_1"/>
      </div>
      <div class="response_image">
        <img id="imgTest_2"/>
      </div>
      <div class="response_image">
        <img id="imgTest_3"/>
      </div>
      <div class="response_image">
        <img id="imgTest_4"/>
      </div>
      <div class="response_image">
        <img id="imgTest_5"/>
      </div>
      <div class="response_image">
        <img id="imgTest_6"/>
      </div>
      <div class="response_image">
        <img id="imgTest_7"/>
      </div>
      <div class="response_image">
        <img id="imgTest_8"/>
      </div>
      <div class="response_image">
        <img id="imgTest_9"/>
      </div>
    </div>


  </div>
</template>

<script>
const ENDPOINT = ''; // set specific URI
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
    async getFile(file_name, num) {
      console.log(file_name)
      let res_get = await axios.get(`${ENDPOINT}/${file_name}`, {
        responseType: 'blob'
      });

      if ( res_get.status === 200) {
        var reader = new FileReader();
        reader.onloadend = function() {
          var img = document.getElementById(`imgTest_${num}`);
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

        for (let i =0; i<10; i++) {
          const file_name_array = this.file.name.split('.')
          const request_file = `${file_name_array[0]}_gen_${i}.png`
          this.getFile(request_file, i)
        }

      } catch (e) {
        throw new Exception(e)
      }
    }
  }
}
</script>

<style>
  .main{
    width:80%;
    margin: 50px auto;
    text-align:left;
    /* border: 1px solid green; */
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
  .main_all_response_image{
    margin:10px 0px;
    width: 100%;
    /* border:1px solid blue; */
    overflow: hidden;
  }
  .response_image{
    float: left;
    width:25%;
    /* border:1px solid red; */
  }
  .response_image img{
    width:100%;
    height:100%;
  }
</style>
