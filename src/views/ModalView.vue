
<script setup>
  import CustomModal from '../components/CustomModal.vue'

</script>

<template>
  <div class="modal">
    <h1>This is the Modal Page</h1>

    <CustomModal>
      <template #header>
        <h2>Yawning Title</h2>
      </template>

      <template v-slot:body>
        <p>Main Body part</p>
        <p>Sub body part</p>
      </template>

      <template v-slot:footer>
        <footer>
          <p>logos can be here.</p>
        </footer>
      </template>
    </CustomModal>

     <CustomModal>
      <template #header>
        <h2>Eye is Dim Title</h2>
      </template>

      <template v-slot:body>
        <p>Feeling Sleepy.</p>
        <p>Dozing and hungry.</p>
      </template>

      <template v-slot:footer>
        <footer>
          <p>Some serenre can be here.</p>
        </footer>
      </template>
    </CustomModal>

    
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .modal {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
