<template>
  <div class="slide">
    <div class="heading">DIP - Inheritance</div>
    <div class="content">
      <div class="flex-container">
        <div style="width: 58%">
          <h2>Ça sent le désordre</h2>
          <br />
          <p>
            Nous ne pouvons pas étendre plusieurs classes de base dans les
            classes Computer et Lamp.
          </p>
          <p>Nous laissons donc le device étendre InventoryAsset.</p>
          <p>
            Tout ce qui étend maintenant Device est-un (is-a) device et-un
            (is-a) inventoryAsset.
          </p>
          <h3>Le téléphone privé est-il un InventoryAsset?</h3>
        </div>
        <div style="width: 40%">
          <img
            src="../assets/illustrations/buttonDIPextendedInheritanceInventoryMess.svg"
            style="width: 100%"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
