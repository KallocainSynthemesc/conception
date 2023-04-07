<template>
  <div class="slide">
    <div class="heading">DIP - Dependency Inversion Principle</div>
    <div class="content">
      <div class="flex-container">
        <div style="width: 49%">
          <h2>Exercice: Ce code ne suit-il pas le DIP ?</h2>
          <br />
          <p>
            Voyez comment MessageService a deux dépendances pour EmailSender et
            TextMessageSender. Que diriez-vous de modifier le code en respectant
            la règle DIP ?
          </p>
          <a
            href="./exercices/dip/DIP-exercice-2.zip"
            download="DIP-exercice-2.zip"
            ><img
              src="../assets/illustrations/zip-file.svg"
              style="width: 10%"
            />Download zip exercice</a
          >
        </div>
        <div style="width: 50%">
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
          <span style="color: #008800; font-weight: bold">public</span> <span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">MessageService</span> <span style="color: #333333">{</span>
              <span style="color: #008800; font-weight: bold">private</span> EmailSender emailSender<span style="color: #333333">;</span>
              <span style="color: #008800; font-weight: bold">private</span> TextMessageSender textMessageSender<span style="color: #333333">;</span>
              
              <span style="color: #008800; font-weight: bold">public</span> <span style="color: #0066BB; font-weight: bold">MessageService</span><span style="color: #333333">()</span> <span style="color: #333333">{</span>
                  emailSender <span style="color: #333333">=</span> <span style="color: #008800; font-weight: bold">new</span> EmailSender<span style="color: #333333">();</span>
                  textMessageSender <span style="color: #333333">=</span> <span style="color: #008800; font-weight: bold">new</span> TextMessageSender<span style="color: #333333">();</span>
              <span style="color: #333333">}</span>
              
              <span style="color: #008800; font-weight: bold">public</span> <span style="color: #333399; font-weight: bold">void</span> <span style="color: #0066BB; font-weight: bold">sendEmail</span><span style="color: #333333">(</span>String message<span style="color: #333333">)</span> <span style="color: #333333">{</span>
                  emailSender<span style="color: #333333">.</span><span style="color: #0000CC">sendEmail</span><span style="color: #333333">(</span>message<span style="color: #333333">);</span>
              <span style="color: #333333">}</span>
              
              <span style="color: #008800; font-weight: bold">public</span> <span style="color: #333399; font-weight: bold">void</span> <span style="color: #0066BB; font-weight: bold">sendTextMessage</span><span style="color: #333333">(</span>String message<span style="color: #333333">)</span> <span style="color: #333333">{</span>
                  textMessageSender<span style="color: #333333">.</span><span style="color: #0000CC">sendTextMessage</span><span style="color: #333333">(</span>message<span style="color: #333333">);</span>
              <span style="color: #333333">}</span>
          <span style="color: #333333">}</span></pre>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
