<template>
<main class="container">
<form class="form" 
      id="form" 
      action="" 
      method="post" 
      novalidate="true">
<!-- adding jsonbin in the future -->

    <h4>Contact Form</h4>
    <p>Message me to share or collaborate</p>
    <fieldset>
        <div>
            <label>First Name</label>
            <input type="text" name="firstName" reguired v-model="firstName"/>
        </div>
        <div>
            <label>Last Name</label>
            <input type="text" name="lastName" reguired v-model="lastName" />
        </div>

        <div>
            <label>Email</label>
            <input type="email" name="email" required v-model="email"/>
        </div>

        <div>
            <label>Message</label>
            <textarea type="text" name="message" required v-model="message"></textarea>
        </div>

        <div class="submit">
            <button type="submit" @click="handlesubmit()">Submit Form</button>
        </div>
    </fieldset>  
  </form>

  </main>
</template>

<script>
    export default {
        data() {
            return {
                firstName:'',
                lastName:'',
                email: '',
                message:''
            }
        },
        methods: {

            handleSubmit() {
            if (this.firstName = this.firstName.length < 1) {
                alert("First Name must be greater than one characer")
                return;
            }

            if (this.lastName = this.lastName.length < 1) {
                alert("Last Name must be greater than one characer")
                return;
            }

            if (!this.email.includes("@") || !this.email.includes(".")) {
                alert("Please enter a valid email address.");
            }
           

            
            // var form = document.getElementById('form');

            // form.addEventListener('submit', (event) => {
            // event.preventDefault();
            // console.log(Array.from(form.elements).map((el) => {
            // return `${el.name}: ${el.value}`;
            // }))
            // });
            
            // goToHome(){
            //     alert("Thank you for you submission")
            //     this.$router.push('/'); 
            // },
            },
        }
    }
   
    
    
// var form = document.getElementById('form');

// form.addEventListener('submit', (event) => {
// event.preventDefault();
// console.log(Array.from(form.elements).map((el) => {
// return `${el.name}: ${el.value}`;        
</script>

<style>

body {
    font-family: 'Fira sans', sans-serif;
    background: #4158D0;
    background: linear-gradient(
    115deg,
    rgba(86, 216, 228, 1) 10% ,
    rgba(159, 1, 234, 1) 90%);
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}
    
.container {
    display: flex;
    align-content: center;
    justify-content: center;

}

.form {
    width: 25rem;
    margin: 50px auto;
    padding: 15px 30px;
    border-radius: .5rem;
    background:  #fff;
     -webkit-box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12),0 1px 2px rgba(0, 0, 0, 0.24);
    box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12), 0 1px 2px rgba(0, 0, 0, 0.24);  
}

.form fieldset {
    margin: 24px 0 0 0;
    border: none;
}

.form div {
    position: relative;
    margin: 2rem 0;
}

.form h4,
.form .label {
    font-size: 1.4rem;
    margin-bottom: 10px;
}

.form .label {
    display: block;
}

.form input,
.form textarea
.form label {
    font-family: "Open Sans", sans-serif;
    font-size: 1.6rem;
    color: #2b3e51;
}

.form input[type="text"],
.form input[type="email"],
.form textarea {
    display: block;
    width: 100%;
    -webkit-appearance: none;
    -moz-appearance: none;
    appearance: none;
}

.form input[type="text"],
.form input[type="email"],
.form textarea {
    padding: 12px;
    border: 1px solid #cfd9db;
    background-color: #ffffff;
    border-radius: 0.25em;
    -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.08);
    box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.08);
}

.form input[type="text"]:focus,
.form input[type="email"]:focus,
.form textarea:focus {
    outline: none;
    border-color: #2c3e50;
    -webkit-box-shadow: 0 0 5px rgba(44, 151, 222, 0.2);
    box-shadow: 0 0 5px rgba(44, 151, 222, 0.2);
}

.form textarea {
    min-height: 120px;
    resize: vertical;
    overflow: auto;
}

.submit {
    border: none;
    background: #7e7e7e;
    border-radius: 0.25em;
    padding: 12px 20px;
    color: #ffffff;
    font-weight: bold;
    margin:auto;
    text-align: center;
    cursor: pointer;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    -webkit-appearance: none;
    -moz-appearance: none;
    appearance: none;
}

.error {
    font-size: 12px;
}


</style>