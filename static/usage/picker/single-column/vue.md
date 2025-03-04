```html
<template>
  <ion-content class="ion-padding">
    <ion-button @click="openPicker()">Open</ion-button>
  </ion-content>
</template>

<script>
  import { IonButton, IonContent, pickerController } from '@ionic/vue';
  import { defineComponent } from 'vue';

  export default defineComponent({
    components: { IonButton, IonContent },
    data() {
      return {
        message: '',
      };
    },
    methods: {
      async openPicker() {
        const picker = await pickerController.create({
          columns: [
            {
              name: 'languages',
              options: [
                {
                  text: 'JavaScript',
                  value: 'javascript',
                },
                {
                  text: 'TypeScript',
                  value: 'typescript',
                },
                {
                  text: 'Rust',
                  value: 'rust',
                },
                {
                  text: 'C#',
                  value: 'c#',
                },
              ],
            },
          ],
          buttons: [
            {
              text: 'Cancel',
              role: 'cancel',
            },
            {
              text: 'Confirm',
              handler: (value) => {
                window.alert(`You selected: ${value.languages.value}`);
              },
            },
          ],
        });
        await picker.present();
      },
    },
  });
</script>
```
