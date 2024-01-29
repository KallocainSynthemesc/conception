<template>
  <div class="slide">
    <div class="heading">Business Logic Layer - Validation</div>
    <div class="content">
      <p>
        Pas assez d'annotations ? Pas grave, puisque nous pouvons faire nos
        propres validations.
      </p>
      <h3>Exemple avec notre personne</h3>
      <div class="flex-container">
        <div style="width: 50%">
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
            <span style="color: #555555; font-weight: bold">@Target</span><span style="color: #333333">({</span> METHOD<span style="color: #333333">,</span> FIELD<span style="color: #333333">,</span> ANNOTATION_TYPE <span style="color: #333333">})</span>
            <span style="color: #555555; font-weight: bold">@Retention</span><span style="color: #333333">(</span>RUNTIME<span style="color: #333333">)</span>
            <span style="color: #555555; font-weight: bold">@Constraint</span><span style="color: #333333">(</span>validatedBy <span style="color: #333333">=</span> AdultValidator<span style="color: #333333">.</span><span style="color: #0000CC">class</span><span style="color: #333333">)</span>
            <span style="color: #555555; font-weight: bold">@Documented</span>
            <span style="color: #008800; font-weight: bold">public</span> <span style="color: #555555; font-weight: bold">@interface</span> Adult <span style="color: #333333">{</span>

                String <span style="color: #0066BB; font-weight: bold">message</span><span style="color: #333333">()</span> <span style="color: #008800; font-weight: bold">default</span> <span style="background-color: #fff0f0">&quot;Vous devez être&quot;</span>
            <span style="color: #333333">+</span><span style="background-color: #fff0f0">&quot;âgé d&#39;au moins 18 ans&quot;</span><span style="color: #333333">;</span>

                Class<span style="color: #333333">&lt;?&gt;[]</span> groups<span style="color: #333333">()</span> <span style="color: #008800; font-weight: bold">default</span> <span style="color: #333333">{};</span>

                Class<span style="color: #333333">&lt;?</span> <span style="color: #008800; font-weight: bold">extends</span> Payload<span style="color: #333333">&gt;[]</span> payload<span style="color: #333333">()</span> <span style="color: #008800; font-weight: bold">default</span> <span style="color: #333333">{};</span>

            <span style="color: #333333">}</span></pre>
          </div>
        </div>
        <div style="width: 50%">
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
            <span style="color: #008800; font-weight: bold">public</span> <span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">AdultValidator</span> <span style="color: #008800; font-weight: bold">implements</span>
                ConstraintValidator<span style="color: #333333">&lt;</span>Adult<span style="color: #333333">,</span> Integer<span style="color: #333333">&gt;</span> <span style="color: #333333">{</span>

                <span style="color: #008800; font-weight: bold">public</span> <span style="color: #333399; font-weight: bold">void</span> <span style="color: #0066BB; font-weight: bold">initialize</span><span style="color: #333333">(</span>Adult constraint<span style="color: #333333">)</span> <span style="color: #333333">{</span>
                <span style="color: #333333">}</span>

                <span style="color: #008800; font-weight: bold">public</span> <span style="color: #333399; font-weight: bold">boolean</span> <span style="color: #0066BB; font-weight: bold">isValid</span><span style="color: #333333">(</span>Integer age<span style="color: #333333">,</span>
                ConstraintValidatorContext context<span style="color: #333333">)</span> <span style="color: #333333">{</span>
                    <span style="color: #008800; font-weight: bold">if</span> <span style="color: #333333">(</span>age <span style="color: #333333">==</span> <span style="color: #008800; font-weight: bold">null</span><span style="color: #333333">)</span> <span style="color: #333333">{</span>
                        <span style="color: #008800; font-weight: bold">return</span> <span style="color: #008800; font-weight: bold">false</span><span style="color: #333333">;</span>
                    <span style="color: #333333">}</span>
                    <span style="color: #008800; font-weight: bold">return</span> age <span style="color: #333333">&gt;=</span> <span style="color: #0000DD; font-weight: bold">18</span><span style="color: #333333">;</span>
                <span style="color: #333333">}</span>
            <span style="color: #333333">}</span></pre>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
