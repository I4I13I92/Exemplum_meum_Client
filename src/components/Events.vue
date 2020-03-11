<template>
	<div id="Events" class="aries-background">
		<input type="" name="" v-model="activity" placeholder="Enter your activity, reading, lifting, etc...">
		<input type="" name="" v-model="duration" placeholder="Enter time in minutes">
		<button @click='Post_Upload()'>Post Upload</button>
	</div>
</template>
<script>
import axios from 'axios'
export default{
	data() {
		return {
			duration: '',
			activity: ''
		}
	},
	methods: {
		Post_Upload(){
			axios.post('http://localhost:8081/astroserver', {
				duration: this.duration,
				activity: this.activity
			})
			.then(res => {
				console.log(res.data.curr_act)
				this.duration = '';
				this.activity = '';
			})

		}
	}

}
</script>

<style>
	.aries-background{
		background-image: url('../assets/ariesSun.jpg');
        background-size: contain;
	}
</style>