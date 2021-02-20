<template>
  <div>
    <nav class="navbar navbar-expand-sm bg-dark navbar-dark justify-content-end py-0">
      <ul class="navbar-nav">

        <li class="nav-item ">
          <div class="nav-link register clickable">
            Register
          </div>
        </li>

        <li class="nav-item" >
          <div class="nav-link clickable">
            Login
          </div>
        </li>
        <li class="nav-item" >
          <div class="nav-link clickable">
            Logout
          </div>
        </li>
        <li class="nav-item" >
          <div class="nav-link clickable">
            Aaa
          </div>
        </li>
      </ul>
    </nav>
    <login-dialog
      :visible.sync="loginDialogVisible"
      :default-tab="defaultLoginDialogTab"
    >
    </login-dialog>
  </div>
</template>

<script>
import LoginDialog from '../components/user/Login'
// import { makeLogout } from '../services/auth.service'
// import { mapGetters } from 'vuex'

export default {

  components: {
    LoginDialog
  },

  data () {
    return {
      makeLogout,
      loginDialogVisible: false,
      defaultLoginDialogTab: 'login',
      value: '',
    //   tours: []
    }
  },

  computed: {
    greeting () {
      return `Hello ${this.$currentUser.email}`
    }
  }
}
</script>

<style lang="stylus" scoped>
</style>
