<template>
  <div class="slide">
    <div class="heading">Inheritance - composition au lieu de l'héritage</div>
    <div class="content">
      <h2>Ce qui s'est passé?</h2>
      <p>
        En interne, la méthode addAll de HashSet est implémentée au-dessus de la
        méthode add. HashSet ne documente pas ce détail d'implémentation.
      </p>
      <h2>Options?</h2>
      <br />
      <h3>Pas de surcharge de addAll</h3>
      <p>
        <span style="font-size: 2rem">↪</span> le fait que addAll utilise sa
        méthode interne "add" peut changer, ce qui casserait à nouveau notre
        classe
      </p>
      <br />
      <h3>
        Surcharge la méthode addAll pour itérer sur la collection spécifiée, en
        appelant la méthode "add" une fois pour chaque élément
      </h3>
      <p>
        <span style="font-size: 2rem">↪</span> n'est pas toujours possible car
        certaines méthodes ne peuvent être implémentées sans accès à des champs
        privés inaccessibles à la sous-classe.
      </p>
    </div>
  </div>
</template>

<style scoped></style>
