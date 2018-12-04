<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js + TypeScript App"/>
		<!-- <md-button>click me</md-button> -->
		      <mt-field  placeholder="请输入密码"  type="password" v-model="upass" class="myinput"></mt-field>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

// import HelloWorld from '@/components/HelloWorld.vue'; // @ is an alias to /src
import HelloWorld from '@/views/index.vue';

@Component({
  components: {
    HelloWorld,
  },
})
export default class Home extends Vue {
	data() {
		return {
			upass: ''
		}
	}
}
</script>
