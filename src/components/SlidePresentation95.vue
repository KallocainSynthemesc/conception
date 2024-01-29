<template>
  <div class="slide">
    <div class="heading">Business Logic Layer - Validation</div>
    <div class="content">
      <p>Il existe également des contraintes de méthode :</p>
      <h3>Single Parameter Constraints</h3>
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
        <span style="color: #008800; font-weight: bold">public</span> <span style="color: #333399; font-weight: bold">void</span> <span style="color: #0066BB; font-weight: bold">createReservation</span><span style="color: #333333">(</span><span style="color: #555555; font-weight: bold">@NotNull</span> <span style="color: #555555; font-weight: bold">@Future</span> LocalDate begin<span style="color: #333333">,</span>
          <span style="color: #555555; font-weight: bold">@Min</span><span style="color: #333333">(</span><span style="color: #0000DD; font-weight: bold">1</span><span style="color: #333333">)</span> <span style="color: #333399; font-weight: bold">int</span> duration<span style="color: #333333">,</span> <span style="color: #555555; font-weight: bold">@NotNull</span> Customer customer<span style="color: #333333">)</span> <span style="color: #333333">{</span>

        <span style="color: #888888">// ...</span>
        <span style="color: #333333">}</span></pre>
      </div>
      <br />
      <h3>Return Value Constraints</h3>
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
        <span style="color: #008800; font-weight: bold">public</span> <span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">ReservationManagement</span> <span style="color: #333333">{</span>

            <span style="color: #555555; font-weight: bold">@NotNull</span>
            <span style="color: #555555; font-weight: bold">@Size</span><span style="color: #333333">(</span>min <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">1</span><span style="color: #333333">)</span>
            <span style="color: #008800; font-weight: bold">public</span> List<span style="color: #333333">&lt;</span><span style="color: #555555; font-weight: bold">@NotNull</span> Customer<span style="color: #333333">&gt;</span> getAllCustomers<span style="color: #333333">()</span> <span style="color: #333333">{</span>
                <span style="color: #008800; font-weight: bold">return</span> <span style="color: #008800; font-weight: bold">null</span><span style="color: #333333">;</span>
            <span style="color: #333333">}</span>
        <span style="color: #333333">}</span></pre>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
