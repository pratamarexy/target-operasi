<template>
  <div class="wrapper">
    <div class="animated fadeIn">
      <b-card
        header-tag="header"
        footer-tag="footer">
        <div slot="header">
          <i class="fa fa-align-justify"></i> <strong>Bootstrap </strong>
          <div class="card-actions">
            <a href="https://bootstrap-vue.js.org/docs/components/" target="_blank">
              <small class="text-muted">docs</small>
            </a>
          </div>
        </div>
        <div>
          <b- header="Bootstrap 4" lead="Bootstrap 4 Components for Vue.js 2">
            <p>For more information visit website</p>
            <b-btn variant="primary" href="#">More Info</b-btn>
          </b->
        </div>
      </b-card>
      <b-card
        header-tag="header"
        footer-tag="footer">
        <div slot="header">
          <i class="fa fa-align-justify"></i> <strong></strong>
          <small>with slots</small>
        </div>
        <div>
          <b->
            <template slot="header">
              Bootstrap 4
            </template>
            <template slot="lead">
              This is a simple hero unit, a simple -style component for
              calling extra attention to featured content or information.
            </template>
            <hr class="my-4">
            <p>
              It uses utility classes for typography and spacing to space content
              out within the larger container.
            </p>
            <b-btn variant="primary" href="#">Do Something</b-btn>
            <b-btn variant="success" href="#">Do Something Else</b-btn>
          </b->
        </div>
      </b-card>
      <b-card
        header-tag="header"
        footer-tag="footer">
        <div slot="header">
          <i class="fa fa-align-justify"></i> <strong></strong>
          <small>variants</small>
        </div>
        <div>
          <b- bg-variant="info" text-variant="white" border-variant="dark">
            <template slot="header">
              Bootstrap 4
            </template>
            <template slot="lead">
              This is a simple hero unit, a simple -style component for
              calling extra attention to featured content or information.
            </template>
            <hr class="my-4">
            <p>
              It uses utility classes for typography and spacing to space content
              out within the larger container.
            </p>
          </b->
        </div>
      </b-card>
    </div>
  </div>
</template>

<script>
  export default {
    name: 's'
  }
</script>

<style scoped>

</style>
