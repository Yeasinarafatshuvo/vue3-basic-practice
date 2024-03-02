<template>
<form @submit.prevent="submitForm">
    <div>
      <label for="name">Name:</label>
      <input type="text" id="name" v-model="formData.name" >
      <span v-if="errors.name" class="error">{{ errors.name }}</span>
    </div>
    <div>
      <label for="email">Email:</label>
      <input type="email" id="email" v-model="formData.email" >
      <span v-if="errors.email" class="error">{{ errors.email }}</span>
    </div>
    <div>
      <label for="password">Password:</label>
      <input type="password" id="password" v-model="formData.password" >
      <span v-if="errors.password" class="error">{{ errors.password }}</span>
    </div>
    <div>
      <label for="gender">Gender:</label>
      <select id="gender" v-model="formData.gender" >
        <option value="">Select gender</option>
        <option value="male">Male</option>
        <option value="female">Female</option>
        <option value="other">Other</option>
      </select>
      <span v-if="errors.gender" class="error">{{ errors.gender }}</span>
    </div>
    <div>
      <label>Interests:</label>
      <div>
        <input type="radio" id="music" value="music" v-model="formData.interest" >
        <label for="music">Music</label>
      </div>
      <div>
        <input type="radio" id="movies" value="movies" v-model="formData.interest" >
        <label for="movies">Movies</label>
      </div>
      <div>
        <input type="radio" id="books" value="books" v-model="formData.interest" >
        <label for="books">Books</label>
      </div>
      <span v-if="errors.interest" class="error">{{ errors.interest }}</span>
    </div>
    <div>
      <input type="checkbox" id="agree" v-model="formData.agree" >
      <label for="agree">I agree to the terms and conditions</label>
      <span v-if="errors.agree" class="error">{{ errors.agree }}</span>
    </div>
    <div>
      <button type="submit">Submit</button>
    </div>
  </form>
</template>

<script>
export default{
    name:"Home",
    components:{
        
    },
    data(){
        return{
            formData: {
                name: '',
                email: '',
                password: '',
                gender: '',
                interest: '',
                agree: false
            },
            errors: {}
        }
    },
    methods:{
        submitForm(){
            this.errors = {};
            if (!this.formData.name) {
        this.errors.name = 'Name is required.';
      }
      if (!this.formData.email) {
        this.errors.email = 'Email is required.';
      } else if (!this.validateEmail(this.formData.email)) {
        this.errors.email = 'Invalid email format.';
      }
      if (!this.formData.password) {
        this.errors.password = 'Password is required.';
      } else if (this.formData.password.length < 6) {
        this.errors.password = 'Password must be at least 6 characters long.';
      }
      if (!this.formData.gender) {
        this.errors.gender = 'Gender is required.';
      }
      if (!this.formData.interest) {
        this.errors.interest = 'Interest is required.';
      }
      if (!this.formData.agree) {
        this.errors.agree = 'You must agree to the terms and conditions.';
      }
      
      // If there are no errors, you can proceed with form submission
      if (Object.keys(this.errors).length === 0) {
        // Perform form submission or other actions here
        console.log('Form submitted successfully!');
        console.log(this.formData);
      }
        },
        validateEmail(email){
            const re = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;

            return re.test(email);
        }
    }
}
</script>


<style scoped>
.green{
    color:green
}
</style>