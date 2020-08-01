<template>
  <div>
    <v-expand-transition>
      <div v-if="show">
        <v-alert :type="type" text>{{ message }}</v-alert>
      </div>
    </v-expand-transition>

    <v-btn color="success" outlined @click="onClickSuccess">success</v-btn>
    <v-btn color="error" outlined @click="onClickError">error</v-btn>
  </div>
</template>

<script lang="ts">
export default {
  data: () => ({
    show: false,
    type: '',
    message: ''
  }),
  methods: {
    onClickSuccess() {
      this.type = 'success'
      this.message = "I'm a success alert."
      this.show = true
      setTimeout(this.onShowFalse, 5000)
    },
    onClickError() {
      this.type = 'error'
      this.message = "I'm an error alert."
      this.show = true
      setTimeout(this.onShowFalse, 5000)
    },
    onShowFalse() {
      this.show = false
    }
  }
}
</script>
