<template>
  <v-dialog v-model="dialog" persistent max-width="600px">
      <v-card>
        TESTE
        
        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn color="blue darken-1" text @click="closeDialog">
            Close
          </v-btn>
          <v-btn color="blue darken-1" text @click="save">
            Save
          </v-btn>
        </v-card-actions>

      </v-card>
  </v-dialog>
</template>

<script>
  export default {
    props: {
      dialog: {
        type: Boolean,
        require: true
      },
      closeDialog: {
        type: Function,
        required: true
      },
      save: {
        type: Function,
        required: true
      }
    }
  }
</script>