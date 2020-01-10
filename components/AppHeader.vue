<template>
  <b-navbar toggleable="lg" type="dark" variant="dark">
    <b-navbar-brand href="#">Simple Ecommerce</b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse class="justify-content-end" id="nav-collapse" is-nav>
      <b-navbar-nav class="ml-auto">
        <b-nav-item class="m-auto" href="#">Home</b-nav-item>
        <b-nav-item href="#">Categories</b-nav-item>
        <b-nav-item href="#">Product</b-nav-item>
        <b-nav-item href="#">Cart</b-nav-item>
        <b-nav-item href="#">Contact</b-nav-item>
      </b-navbar-nav>

      <b-navbar-nav class="ml-auto">
        <b-nav-form class="my-2 my-lg-0">
          <b-input-group size="sm">
            <b-form-input placeholder="Search..."></b-form-input>
            <b-input-group-prepend>
              <b-button>
                <Fas i="search"/>
              </b-button>
            </b-input-group-prepend>
          </b-input-group>

          <b-button class="ml-3" href="cart.html" variant="success" size="sm">
            <Fas i="shopping-cart"/>
            <span class="badge badge-light">3</span>
          </b-button>
        </b-nav-form>

        <b-nav-item-dropdown text="Lang" right>
          <b-dropdown-item href="#">EN</b-dropdown-item>
          <b-dropdown-item href="#">ES</b-dropdown-item>
          <b-dropdown-item href="#">RU</b-dropdown-item>
          <b-dropdown-item href="#">FA</b-dropdown-item>
        </b-nav-item-dropdown>

        <b-nav-item-dropdown right>
          <!-- Using 'button-content' slot -->
          <template v-slot:button-content>
            <em>User</em>
          </template>
          <b-dropdown-item href="#">Profile</b-dropdown-item>
          <b-dropdown-item href="#">Sign Out</b-dropdown-item>
        </b-nav-item-dropdown>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<script>
  import Fas from "./Fas";

  export default {
    name: "AppHeader",
    components: {
      Fas
    }
  }
</script>

<style scoped>

</style>
