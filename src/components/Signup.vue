<template>
	<div id="signup">
        <img alt="logo" src="../assets/logo.png" style="margin-bottom: 50px; margin-top: 50px;"/>
		<form @submit.prevent="submitForm">
            <h4 style="background-color: #9beacd;">PLEASE SIGNUP TO CONTINUE</h4>
			<div style="margin-top: 15px;">
				<div for="email" text-align="left" style="margin-right: 500px; ">email</div>
				<input type="text" class="w3-input" id="user_email" name="user_email" v-model="user_email" placeholder="Enter your email"/>
			</div>
			<div style="margin-top: 15px;">
				<div for="name" style="margin-right: 500px; ">name</div>
				<input type="text" class="w3-input" id="user_name" name="user_name" v-model="user_name" placeholder="Enter your name" />
			</div>
			<div style="margin-top: 15px;">
				<div for="password" style="margin-right: 500px; ">password</div>
				<input type="password" class="w3-input" id="user_password" name="user_password" v-model="user_password" placeholder="Enter your password"/>
			</div>
			<div style="margin-top: 15px;">
				<div for="passwordConfirm" style="margin-right: 380px; white-space : nowrap ">password Confirm</div>
				<input type="password" class="w3-input" id="user_passwordConfirm" name="user_passwordConfirm" v-model="user_passwordConfirm" placeholder="Confirm your Password"/>
			</div>
			<div style="margin-top: 15px;">
				<div for="position" text-align="left" style="margin-right: 500px; ">phonecall</div>
				<input type="text" class="w3-input" id="user_phone" name="user_phone" v-model="position" placeholder="Enter your phone number"/>
			</div>
			<button type="submit" class="w3-button w3-round" style="background-color: #9beacd; margin-top: 12px; margin-bottom: 70px;">SIGNUP</button>
		</form>
	</div>
</template>

<script>
export default {
	name: 'SignupForm',
	data() {
		return {
			user_email: '',
			user_name: '',
			user_password: '',
			user_passwordConfirm: '',
			user_phone: '',
		};
	},
	methods: {
		submitForm() {
			console.log('dd');
		},
	},
};
</script>

<style scoped>
 @import "https://www.w3schools.com/w3css/4/w3.css";
 #signup {
    width: 500px;
    margin: auto;
  }
</style>