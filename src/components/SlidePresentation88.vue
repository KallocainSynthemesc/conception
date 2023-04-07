<template>
  <div class="slide">
    <div class="heading">Business Logic Layer</div>
    <div class="content">
      <h2>Indications</h2>
      <p>
        Certaines classes et interfaces doivent être modifiées. Plus important
        encore, nous devons développer le BankAccountDAO. PersonService doit
        maintenant être en mesure de supprimer des personnes et des comptes
        bancaires. Bonne chance !
      </p>
      <div class="flex-container">
        <div style="width: 39%">
          <h3>PersonService</h3>
          <div
            style="
              background: #ffffff;
              overflow: auto;
              width: auto;
              border: solid gray;
              border-width: 0.1em 0.1em 0.1em 0.8em;
              padding: 0.2em 0.6em;
            "
          >
            <pre style="margin: 0; line-height: 125%">
            public <span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">PersonService</span>{
	
              final PersonDAO dao;
              final BankAccountDAO bankAccDao;

              public void remove(Person person) {
                  <span style="color: #333333">...</span>
              }
            }</pre>
          </div>
          <a
            href="/conception/exercices/service/Service-exercice-1.zip"
            download="Service-exercice-1.zip"
            ><img
              src="../assets/illustrations/zip-file.svg"
              style="width: 10%"
            />Download zip exercice</a
          >
        </div>
        <div style="width: 59%">
          <h3>BankAccountDAO</h3>
          <div
            style="
              background: #ffffff;
              overflow: auto;
              width: auto;
              border: solid gray;
              border-width: 0.1em 0.1em 0.1em 0.8em;
              padding: 0.2em 0.6em;
            "
          >
            <pre style="margin: 0; line-height: 125%">
            <span style="color: #008800; font-weight: bold">public</span> <span style="color: #008800; font-weight: bold">interface</span> <span style="color: #BB0066; font-weight: bold">BankAccountDAO</span> <span style="color: #333333">{</span>
     
                <span style="color: #008800; font-weight: bold">public</span> BankAccount <span style="color: #0066BB; font-weight: bold">findByAccountOwner</span><span style="color: #333333">(</span>Person owner<span style="color: #333333">);</span>
                
                <span style="color: #008800; font-weight: bold">public</span> BankAccount <span style="color: #0066BB; font-weight: bold">findByConsultant</span><span style="color: #333333">(</span>Person consultant<span style="color: #333333">);</span>

                <span style="color: #333333">...</span>
            <span style="color: #333333">}</span></pre>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
