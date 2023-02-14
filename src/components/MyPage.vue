<template id = "body">
    <div id="Mypage">
        <div>
            <img alt="logo" src="../assets/logo.png" style="margin-bottom: 50px; margin-top: 50px;" />
            <form @submit.prevent="submitForm">
            <h4 style="background-color: #9beacd;">My Page</h4>
            <div style="margin-top: 15px;">
                <div for="email" text-align="left" style="margin-right: 500px; ">email</div>
                <input type="text" class="w3-input" id="email" v-model="user_email" placeholder="이메일" />
            </div>
            <div style="margin-top: 15px;">
                <div for="name" style="margin-right: 500px; ">name</div>
                <input type="text" class="w3-input" id="name" v-model="user_name" placeholder="이름" />
            </div>

            <div style="margin-top: 15px;">
                <div for="position" text-align="left" style="margin-right: 500px; ">phonecall</div>
                <input type="text" class="w3-input" id="phone" v-model="position" placeholder="폰번호" />
            </div>
            <button type="submit" class="w3-button w3-round"
                    style="background-color: #9beacd; margin-top: 12px; margin-bottom: 70px;">MODIFY
            </button>
            </form>
            <h4 style="background-color: #9beacd; margin-bottom: 30px;">my favor</h4>
        </div>
        
    </div>


</template>

<script>
export default {
    name: 'SignupForm',
    data() {
        return {
            email: '',
            name: '',
            password: '',
            passwordConfirm: '',
            phone: '',
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


#Mypage {
    width: 500px;
    margin: auto;
}


</style>