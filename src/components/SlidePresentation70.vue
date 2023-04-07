<template>
  <div class="slide">
    <div class="heading">Historique - j2ee Architecture</div>
    <div class="content">
      <div class="flex-container">
        <div style="width: 50%">
          <h3>Web container (ou Servlet container)</h3>
          <p>
            <span style="font-size: 1.6rem">↪</span> Les servlets et les JSP
            fournissent des mécanismes pour la préparation dynamique du contenu,
            et le formatage liés à la présentation.
          </p>
          <h3>Applet container</h3>
          <p>
            <span style="font-size: 1.6rem">↪</span> Complètement mort depuis
            Java 11
          </p>
          <h3>Application client container</h3>
          <p>
            <span style="font-size: 1.6rem">↪</span> semi mort depuis Java 11
            (JNLP, openwebstart)
          </p>
          <h3>EJB container</h3>
          <p>
            <span style="font-size: 1.6rem">↪</span> Les composants EJB, ou
            enterprise beans, sont de deux types : les session beans et les
            entity beans.
          </p>
        </div>
        <div style="width: 50%">
          <img
            src="../assets/illustrations/container.svg"
            style="width: 100%"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
