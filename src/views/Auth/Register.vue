<template>
    <div class="container">
        <div class="columns">
            <div class="column is-6 is-offset-3">
                <h3 class="title is-3">Create account</h3><hr>
                <form action="#" @submit.prevent="register">
                    <div class="field">
                        <label class="label">Name</label>
                        <div class="control">
                          <input class="input" type="text" placeholder="e.g Alex Smith" v-model="name">
                        </div>
                      </div>
                      
                      <div class="field">
                        <label class="label">Email</label>
                        <div class="control">
                          <input class="input" type="email" placeholder="e.g. alexsmith@gmail.com" v-model="email">
                        </div>
                      </div>

                      <div class="field">
                            <label class="label">Password</label>
                            <div class="control">
                              <input class="input" type="password" v-model="password">
                            </div>
                          </div>
                          <button type="submit" class="button is-primary">Register</button>
                </form>
                <div class="notification is-danger" v-if="error">
                   {{ error }} 
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  data() {
    return {
      name: '',
      email: '',
      password: '',
      error: ''
    }
  },
    name: 'Register',
    methods: {
        register(){
          if(name && email){
              //Send form
          }else{
            //Send Error
            this.error = 'Missing data in register!'
          }   
        }
    }
}
</script>