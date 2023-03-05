<template>
  <v-navigation-drawer expand-on-hover rail>
    <v-list>
      <v-list-item
        prepend-avatar="https://randomuser.me/api/portraits/lego/5.jpg"
        title="Ravi Rathod"
        subtitle="ravirathod4449@gmail.com"
      ></v-list-item>
    </v-list>

    <v-divider></v-divider>

    <v-list density="compact" nav>
      <v-list-item
        prepend-icon="mdi-image"
        title="Color Gallery"
        value="color"
        @click="$emit('selectOption', true)"

      ></v-list-item>
      <v-list-item
        prepend-icon="mdi-dialpad"
        title="GreySpace Gallery"
        value="greyspace"
        @click="$emit('selectOption', false)"
      ></v-list-item>
    </v-list>
  </v-navigation-drawer>
</template>
