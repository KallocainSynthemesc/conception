<template>
  <div class="slide">
    <div class="heading">Architectural Component Layer/ Utilities</div>
    <div class="content">
      <p>
        Nous pouvons maintenant utiliser notre validateur sur l'âge des
        personnes.
      </p>
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
    
            <span style="color: #555555; font-weight: bold">@Adult</span>
            <span style="color: #008800; font-weight: bold">private</span> <span style="color: #333399; font-weight: bold">int</span> age<span style="color: #333333">;</span>
            <span style="color: #333333">...</span>
        <span style="color: #333333">}</span></pre>
      </div>
      <p>
        Pour vérifier manuellement la validation, nous devons procéder comme
        suit. (Beaucoup de frameworks font cette étape pour nous)
      </p>
      <!-- HTML generated using hilite.me -->
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
        Person person4 <span style="color: #333333">=</span> <span style="color: #008800; font-weight: bold">new</span> Person<span style="color: #333333">(</span><span style="color: #0000DD; font-weight: bold">4L</span><span style="color: #333333">,</span><span style="background-color: #fff0f0">&quot;John&quot;</span><span style="color: #333333">,</span> <span style="background-color: #fff0f0">&quot;Doe&quot;</span><span style="color: #333333">,</span> <span style="color: #0000DD; font-weight: bold">17</span><span style="color: #333333">);</span>
        ValidatorFactory factory <span style="color: #333333">=</span> Validation<span style="color: #333333">.</span><span style="color: #0000CC">buildDefaultValidatorFactory</span><span style="color: #333333">();</span>
        Validator validator <span style="color: #333333">=</span> factory<span style="color: #333333">.</span><span style="color: #0000CC">getValidator</span><span style="color: #333333">();</span>
        Set<span style="color: #333333">&lt;</span>ConstraintViolation<span style="color: #333333">&lt;</span>Person<span style="color: #333333">&gt;&gt;</span> violations <span style="color: #333333">=</span> validator<span style="color: #333333">.</span><span style="color: #0000CC">validate</span><span style="color: #333333">(</span>person4<span style="color: #333333">);</span>
        <span style="color: #008800; font-weight: bold">for</span> <span style="color: #333333">(</span>ConstraintViolation<span style="color: #333333">&lt;</span>Person<span style="color: #333333">&gt;</span> violation <span style="color: #333333">:</span> violations<span style="color: #333333">)</span> <span style="color: #333333">{</span>
            System<span style="color: #333333">.</span><span style="color: #0000CC">out</span><span style="color: #333333">.</span><span style="color: #0000CC">println</span><span style="color: #333333">(</span>violation<span style="color: #333333">.</span><span style="color: #0000CC">getMessage</span><span style="color: #333333">());</span>
        <span style="color: #333333">}</span></pre>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
