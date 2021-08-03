<template>
  <div class="hello">
		<GlitchedWriter tag="h1" :text="msg" appear />
		<GlitchedWriter tag="p" :text="paragraph" :options="{html:true}" appear />
  </div>
</template>

<script>
import GlitchedWriter from 'vue-glitched-writer'

export default {
  name: 'HelloWorld',
  components: {
    GlitchedWriter
  },
  props: {
    msg: String
  },
  setup(){
		const paragraph = `
		For a guide and recipes on how to configure / customize this project, <br/>
      check out the <a href="https://github.com/thetarnav/vue-glitched-writer" target="_blank">vue glitched writer repo</a>.`

		return {
			paragraph
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
