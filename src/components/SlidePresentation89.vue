<template>
  <div class="slide">
    <div class="heading">Business Logic Layer - Validation</div>
    <div class="content">
      <h2>Validation</h2>
      <p>
        La validation est normalement effectuée sur le VO/DTO/modèle. Dans ce
        cas, notre Value Object layer et notre Business Logic layer se
        chevauchent. Ce n'est pas grave. La validation d'un objet doit être
        proche de l'endroit où il est défini.
      </p>
      <h3>Examinons un exemple simple d'une telle validation</h3>
      <div style="overflow-y: scroll; height: 75%">
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
          <span style="color: #008800; font-weight: bold">public</span> <span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">Person</span> <span style="color: #333333">{</span>
              <span style="color: #008800; font-weight: bold">private</span> <span style="color: #333399; font-weight: bold">long</span> personNum<span style="color: #333333">;</span>
              <span style="color: #008800; font-weight: bold">private</span> String firstName<span style="color: #333333">;</span>
              <span style="color: #008800; font-weight: bold">private</span> String lastName<span style="color: #333333">;</span>
              <span style="color: #008800; font-weight: bold">private</span> String socialSecurityNumber<span style="color: #333333">;</span>
  
              <span style="color: #008800; font-weight: bold">public</span> <span style="color: #0066BB; font-weight: bold">Person</span><span style="color: #333333">(</span><span style="color: #333399; font-weight: bold">long</span> personNum<span style="color: #333333">,</span> String firstName<span style="color: #333333">,</span> String lastName<span style="color: #333333">,</span> String socialSecurityNumber<span style="color: #333333">)</span> <span style="color: #333333">{</span>
                  <span style="color: #008800; font-weight: bold">this</span><span style="color: #333333">.</span><span style="color: #0000CC">personNum</span> <span style="color: #333333">=</span> personNum<span style="color: #333333">;</span>
                  <span style="color: #008800; font-weight: bold">this</span><span style="color: #333333">.</span><span style="color: #0000CC">firstName</span> <span style="color: #333333">=</span> firstName<span style="color: #333333">;</span>
                  <span style="color: #008800; font-weight: bold">this</span><span style="color: #333333">.</span><span style="color: #0000CC">lastName</span> <span style="color: #333333">=</span> lastName<span style="color: #333333">;</span>
                  <span style="color: #008800; font-weight: bold">this</span><span style="color: #333333">.</span><span style="color: #0000CC">socialSecurityNumber</span> <span style="color: #333333">=</span> socialSecurityNumber<span style="color: #333333">;</span>
                  validateSocialSecurityNumber<span style="color: #333333">(</span>socialSecurityNumber<span style="color: #333333">);</span>
              <span style="color: #333333">}</span>
  
              <span style="color: #008800; font-weight: bold">private</span> <span style="color: #333399; font-weight: bold">void</span> <span style="color: #0066BB; font-weight: bold">validateSocialSecurityNumber</span><span style="color: #333333">(</span>String socialSecurityNumber<span style="color: #333333">)</span> <span style="color: #333333">{</span>
                  <span style="color: #008800; font-weight: bold">if</span> <span style="color: #333333">(</span>socialSecurityNumber <span style="color: #333333">==</span> <span style="color: #008800; font-weight: bold">null</span> <span style="color: #333333">||</span> <span style="color: #333333">!</span>socialSecurityNumber<span style="color: #333333">.</span><span style="color: #0000CC">matches</span><span style="color: #333333">(</span><span style="background-color: #fff0f0">&quot;\\d{3}-\\d{2}-\\d{4}&quot;</span><span style="color: #333333">))</span> <span style="color: #333333">{</span>
                      <span style="color: #008800; font-weight: bold">throw</span> <span style="color: #008800; font-weight: bold">new</span> <span style="color: #0066BB; font-weight: bold">IllegalArgumentException</span><span style="color: #333333">(</span><span style="background-color: #fff0f0">&quot;Le numéro de sécurité sociale doit être au format ###-##-####.&quot;</span><span style="color: #333333">);</span>
                  <span style="color: #333333">}</span>
              <span style="color: #333333">}</span>
              <span style="color: #888888">// getters et setters omis par souci de concision</span>
          <span style="color: #333333">}</span></pre>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
