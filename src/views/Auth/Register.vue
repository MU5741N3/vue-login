<template>
    <div class="container">
        <div class="columns">
            <div class="column is-6 is-offset-3">
                <h3 class="title is-3">Create account</h3><hr>
                <form action="#" @submit.prevent="register">
                    <div class="field">
                        <label class="label">Name</label>
                        <div class="control">
                          <input class="input" type="text" placeholder="e.g Alex Smith">
                        </div>
                      </div>
                      
                      <div class="field">
                        <label class="label">Email</label>
                        <div class="control">
                          <input class="input" type="email" placeholder="e.g. alexsmith@gmail.com">
                        </div>
                      </div>

                      <div class="field">
                            <label class="label">Password</label>
                            <div class="control">
                              <input class="input" type="password">
                            </div>
                          </div>
                          <button type="submit" class="button is-primary">Register</button>
                </form>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
    name: 'Register',
    methods: {
        register(){
            const Swal = require('sweetalert2')
            Swal.fire(
              'Good job!',
              'You clicked the button!',
              'success'
            )   
        }
    }
}
</script>