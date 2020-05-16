<template>
  <v-list flat subheader>
    <v-subheader>設定</v-subheader>

    <v-list-item-group>
      <v-list-item>
        <v-list-item-action>
          <v-switch v-model="$vuetify.theme.dark" primary></v-switch>
        </v-list-item-action>

        <v-list-item-content>
          <v-list-item-title>ダークモード</v-list-item-title>
        </v-list-item-content>
      </v-list-item>

      <v-list-item>
        <v-list-item-action>
          <v-switch v-model="value"></v-switch>
        </v-list-item-action>

        <v-list-item-content>
          <v-list-item-title>＊＊＊</v-list-item-title>
        </v-list-item-content>
      </v-list-item>

      <v-list-item>
        <v-list-item-action>
          <v-switch v-model="value"></v-switch>
        </v-list-item-action>

        <v-list-item-content>
          <v-list-item-title>＊＊＊</v-list-item-title>
        </v-list-item-content>
      </v-list-item>

      <v-list-item>
        <v-list-item-action>
          <v-switch v-model="value"></v-switch>
        </v-list-item-action>

        <v-list-item-content>
          <v-list-item-title>＊＊＊</v-list-item-title>
        </v-list-item-content>
      </v-list-item>
    </v-list-item-group>
  </v-list>
</template>

<script>
export default {}
</script>
