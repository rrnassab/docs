<template>
  <div class="text-xs-center">
    <v-menu offset-y>
      <v-btn primary light slot="activator">Dropdown</v-btn>
      <v-list>
        <v-list-item v-for="item in items" :key="item">
          <v-list-tile>
            <v-list-tile-title>{{ item.title }}</v-list-tile-title>
          </v-list-tile>
        </v-list-item>
      </v-list>
    </v-menu>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        items: [
          {
            title: 'Click Me'
          },
          {
            title: 'Click Me'
          },
          {
            title: 'Click Me'
          },
          {
            title: 'Click Me 2'
          }
        ]
      }
    }
  }
</script>
