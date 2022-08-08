<template>
<div>

<div>
  <div class="contact-form-wrapper d-flex justify-content-center">
    <form v-on:submit.prevent="submitForm" class="contact-form">
      <h5 class="title">Contact me</h5>
      <p class="description">Feel free to contact me on
      </p>
      <div>
        <input type="text" class="form-control rounded border-white mb-3 form-input" id="name" placeholder="Name" v-model="form.name" required>
      </div>
      <div>
        <input type="email" class="form-control rounded border-white mb-3 form-input" placeholder="Email" v-model="form.email" required>
      </div>
      <div>
        <textarea id="message" class="form-control rounded border-white mb-3 form-text-area" rows="5" cols="30" placeholder="Message" v-model="form.message" required></textarea>
      </div>
      <div class="submit-button-wrapper btn btn-primary">
        <input type="submit" value="Send">
      </div>
    </form>
  </div>
</div>
  

</div>
</template>
<script>
import axios from 'axios';
export default {
    name: "ContactComponent",
    data() {
        return {
          form: {
            name: "",
            email: "",
            message: "",

          }
        }
    },
    methods: {
      submitForm() {
        axios.post("<backend endpoint>",this.form)
        .then((res) => {
          //perfom success action
          console.log(res);
        })
        .catch((error) => {
          //perfom fail action
          console.log(error);
        }).finally(() => {
          
        })
      }
    }
}
</script>
<style>

.contact-form-wrapper {
  padding: 100px 0;
}

.contact-form {
  padding: 30px 40px;
  background-color: #ffffff;
  border-radius: 12px;
  max-width: 400px;
}

.contact-form textarea {
  resize: none;
}

.contact-form .form-input,
.form-text-area {
  background-color: #f0f4f5;
  height: 50px;
  padding-left: 16px;
}

.contact-form .form-text-area {
  background-color: #f0f4f5;
  height: auto;
  padding-left: 16px;
}

.contact-form .form-control::placeholder {
  color: #aeb4b9;
  font-weight: 500;
  opacity: 1;
}

.contact-form .form-control:-ms-input-placeholder {
  color: #aeb4b9;
  font-weight: 500;
}

.contact-form .form-control::-ms-input-placeholder {
  color: #aeb4b9;
  font-weight: 500;
}

.contact-form .form-control:focus {
  border-color: #f33fb0;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.07), 0 0 8px #f33fb0;
}

.contact-form .title {
  text-align: center;
  font-size: 24px;
  font-weight: 500;
}

.contact-form .description {
  color: #aeb4b9;
  font-size: 14px;
  text-align: center;
}

.contact-form .submit-button-wrapper {
  text-align: center;
}

.contact-form .submit-button-wrapper input {
  border: none;
  border-radius: 4px;
  
  color: white;
  text-transform: uppercase;
  padding: 10px 60px;
  font-weight: 500;
  letter-spacing: 2px;
}

.contact-form .submit-button-wrapper input:hover {
  
}


</style>