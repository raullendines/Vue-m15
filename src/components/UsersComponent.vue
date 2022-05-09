<template>
 <div class="row mt-3 flex-reverse">
       
  </div>
</template>

<script>
import axios from 'axios';
export default {
  data(){
    return {
      baseURL: 'https://dummyapi.io/data/v1/'
    }
  },
  name: 'HelloWorld',
  props: {
    msg: String
  },
  methods: {
    getAllProducts(){
          axios
                .get(this.baseURL)
                .then(response => {
                    this.frutas = response.data
                    console.log(this.frutas)
                })
                .catch( e=> console.log(e))
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
