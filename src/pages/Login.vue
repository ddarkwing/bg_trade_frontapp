<template>
  <q-layout>
    <q-page padding>
      <div class="column" style="height: 30px">
        <div class="col"></div>
      </div>
      <q-page-container>
        <q-page class="flex bg-image flex-center">
          <q-card v-bind:style="$q.screen.lt.sm?{'width': '80%'}:{'width':'30%'}">
            <q-card-section>
              <q-avatar size="103px" class="absolute-center shadow-10">
                <img src="../statics/icons/bithumb.png">
              </q-avatar>
            </q-card-section>
            <q-card-section>
              <div class="text-center q-pt-lg">
                <div class="col text-h6 ellipsis">
                  Log in
                </div>
              </div>
            </q-card-section>
            <q-card-section>
              <q-form
              class="q-gutter-md"
              >
              <q-input
              filled
              v-model="username"
              label="Username"
              lazy-rules
              />

              <q-input
              type="password"
              filled
              v-model="password"
              label="Password"
              lazy-rules

              />

              <div>
                <q-btn label="Login" to="/orders" type="button" color="primary"/>
              </div>
            </q-form>
          </q-card-section>
        </q-card>
      </q-page>
    </q-page-container>
  </q-page>

</q-layout>
</template>

<script>
export default {
  data() {
    return {
      username: 'TeslaHash',
      password: '1234578'
    }
  },
}
</script>

<style>

</style>
