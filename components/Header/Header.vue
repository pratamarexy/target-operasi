<template>
  <header class="app-header navbar">
    <button class="navbar-toggler mobile-sidebar-toggler d-lg-none" type="button" @click="mobileSidebarToggle">
      <span class="navbar-toggler-icon"></span>
    </button>
    <b-link class="navbar-brand" to="#">
      <div class="user-avatar"><img src="/img/pp.png"></div>
      <div class=user-detail>
        <h4>John Doe </h4>
        <p>Online</p>
      </div>
    </b-link>
    <button class="navbar-toggler sidebar-toggler d-md-down-none" type="button" @click="sidebarToggle">
      <span class="navbar-toggler-icon"></span>
    </button>

    <b-navbar-nav class="ml-auto">
      <b-nav-item class="d-md-down-none">
        <img src="/img/ic-bell.svg">
        <b-badge pill variant="danger">5</b-badge>
      </b-nav-item>
      <b-nav-item class="d-md-down-none">
        <img src="/img/ic-setting.svg">
      </b-nav-item>
      <b-nav-item class="d-md-down-none">
        <img src="/img/ic-help.svg">
      </b-nav-item>
    </b-navbar-nav>
  </header>
</template>

<script>
  import HeaderDropdown from './HeaderDropdown.vue'

  export default {
    name: 'c-header',
    components: {
      HeaderDropdown
    },
    methods: {
      sidebarToggle (e) {
        e.preventDefault()
        document.body.classList.toggle('sidebar-hidden')
      },
      sidebarMinimize (e) {
        e.preventDefault()
        document.body.classList.toggle('sidebar-minimized')
      },
      mobileSidebarToggle (e) {
        e.preventDefault()
        document.body.classList.toggle('sidebar-mobile-show')
      },
      asideToggle (e) {
        e.preventDefault()
        document.body.classList.toggle('aside-menu-hidden')
      }
    }
  }
</script>
