<template>
  <div class="slide">
    <div class="heading">Architectural Component Layer/ Utilities</div>
    <div class="content">
      <div class="flex-container">
        <div style="width: 48%">
          <p>Pourquoi ne pas extraire la validation?</p>
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
  <span style="color: #008800; font-weight: bold">public</span> <span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">Utils</span> <span style="color: #333333">{</span>

    <span style="color: #008800; font-weight: bold">public</span> <span style="color: #008800; font-weight: bold">static</span> <span style="color: #333333">&lt;</span>T<span style="color: #333333">&gt;</span> String validate<span style="color: #333333">(</span>T t<span style="color: #333333">)</span> <span style="color: #333333">{</span>
      String message <span style="color: #333333">=</span> <span style="background-color: #fff0f0">&quot;&quot;</span><span style="color: #333333">;</span>
      ValidatorFactory factory <span style="color: #333333">=</span> Validation<span style="color: #333333">.</span><span style="color: #0000CC">buildDefaultValidatorFactory</span><span style="color: #333333">();</span>
          Validator validator <span style="color: #333333">=</span> factory<span style="color: #333333">.</span><span style="color: #0000CC">getValidator</span><span style="color: #333333">();</span>
          Set<span style="color: #333333">&lt;</span>ConstraintViolation<span style="color: #333333">&lt;</span>T<span style="color: #333333">&gt;&gt;</span> violations <span style="color: #333333">=</span> validator<span style="color: #333333">.</span><span style="color: #0000CC">validate</span><span style="color: #333333">(</span>t<span style="color: #333333">);</span>
          <span style="color: #008800; font-weight: bold">for</span> <span style="color: #333333">(</span>ConstraintViolation<span style="color: #333333">&lt;</span>T<span style="color: #333333">&gt;</span> violation <span style="color: #333333">:</span> violations<span style="color: #333333">)</span> <span style="color: #333333">{</span>
            message <span style="color: #333333">+=</span> violation<span style="color: #333333">.</span><span style="color: #0000CC">getMessage</span><span style="color: #333333">();</span>
          <span style="color: #333333">}</span>
          <span style="color: #008800; font-weight: bold">return</span> message<span style="color: #333333">;</span>
    <span style="color: #333333">}</span>
<span style="color: #333333">}</span>
</pre>
          </div>
        </div>
        <div style="width: 48%">
          <p>Voici comment nous pouvons l'appeler</p>
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

      Person person <span style="color: #333333">=</span> <span style="color: #008800; font-weight: bold">new</span> Person<span style="color: #333333">(</span><span style="background-color: #fff0f0">&quot;Kilian&quot;</span><span style="color: #333333">,</span> <span style="background-color: #fff0f0">&quot;Schropp&quot;</span><span style="color: #333333">,</span> <span style="color: #0000DD; font-weight: bold">16</span><span style="color: #333333">);</span>
      <span style="color: #008800; font-weight: bold">final</span> String validationMessage <span style="color: #333333">=</span> Utils<span style="color: #333333">.</span><span style="color: #0000CC">validate</span><span style="color: #333333">(</span>person<span style="color: #333333">);</span>
      </pre>
          </div>
          <br />
          <p>
            Nous pouvons désormais utiliser la validation dans plusieurs couches
            et même dans différents projets, car elle est isolée du reste de
            l'application.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
