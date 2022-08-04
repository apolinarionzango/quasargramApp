<template>
  <q-layout view="lHh Lpr lFf">
    <q-header
    class="bg-white text-grey-10"
    bordered
    >
      <q-toolbar>


        <q-toolbar-title
          class="text-grand-hotel text-bold"
        >
          Quasagram
        </q-toolbar-title>


      </q-toolbar>
    </q-header>
    <q-footer

      class="bg-white"
      bordered
    >

        <q-tabs class="text-grey-10"
        active-color="primary"
        indicator-color="transparent">

          <q-route-tab
            to= "/"
            icon="eva-home-outline"
            label="Home"
            name="home"
          />

          <q-route-tab
            to= "/camera"
            icon="eva-camera-outline"
            label="Camera"
            name="camera"
            />



        </q-tabs>

    </q-footer>

    <!--  remover a tag q-drawer  -->


    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>


export default {
  name: 'MainLayout',

  data () {
    return {

    }
  }
}
</script>

<style lang="sass">
.q-toolbar-title
  text-align: center
  .q-footer
   .q-tab_icon
     font-size: 30px

</style>
