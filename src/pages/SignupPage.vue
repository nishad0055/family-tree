<template>
  <div class="md:hidden sm:block">
    <div class="container mx-auto">
      <h3 class="p-3 m-0 text-gray-600">Family Tree</h3>
      <hr />
      <div class="input-box py-3 m-4">
        <label class="text-base">Family ID:</label>
        <q-input
          color="green"
          filled
          v-model="text"
          label="Write your family ID"
          class="mt-2"
        >
          <template v-slot:prepend>
            <q-icon name="person" color="green" />
          </template>
        </q-input>
      </div>
      <div class="input-box py-3 m-4">
        <label class="text-base" for="">Managers (Only Users:)</label>
        <q-input
          color="green"
          v-model="text"
          filled
          class="mt-2"
          label="Type here"
        >
          <template v-slot:prepend>
            <q-icon name="settings" color="green" />
          </template>
        </q-input>
        <div class="toggle">
          <q-toggle
            v-model="value"
            color="green"
            label="can everyone see this family (public view)"
          />
        </div>
      </div>
      <div class="input-box py-3 m-4">
        <label class="text-base" for="">View Password</label>
        <q-input
          color="green"
          class="mt-2"
          filled
          v-model="text"
          label="Write your view password"
        >
          <template v-slot:prepend>
            <q-icon name="lock" color="green" />
          </template>
        </q-input>
      </div>
    </div>
  </div>
</template>

<script>
import { defineComponent } from "vue";
import { ref } from "vue";

export default defineComponent({
  name: "SignupPage",
  setup() {
    return {
      value: ref(true),
    };
  },
});
</script>

<style></style>
