<template>
  <div class="slide">
    <div class="heading">
      Value Object Layer - Data Transfer Object - Model Layer
    </div>
    <div class="content">
      <div class="flex-container" style="overflow-y: scroll; height: 100%">
        <div style="width: 75%">
          <p>
            En règle générale, une VO/DTO possède des accesseurs et des
            mutateurs, mais pas grand-chose d'autre.
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
            public <span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">Person</span> {
                private <span style="color: #007020">long</span> personNum;
                private String firstName;
                private String lastName;
                private List<span style="color: #333333">&lt;</span>String<span style="color: #333333">&gt;</span> phoneNumbers <span style="color: #333333">=</span> new ArrayList<span style="color: #333333">&lt;</span>String<span style="color: #333333">&gt;</span>();

                public Person() {}
                
                public Person(<span style="color: #007020">long</span> personNum, String firstName, String lastName) {
                    <span style="color: #007020">super</span>();
                    this<span style="color: #333333">.</span>personNum <span style="color: #333333">=</span> personNum;
                    this<span style="color: #333333">.</span>firstName <span style="color: #333333">=</span> firstName;
                    this<span style="color: #333333">.</span>lastName <span style="color: #333333">=</span> lastName;
                }

                public <span style="color: #007020">long</span> getPersonNum() {
                    <span style="color: #008800; font-weight: bold">return</span> personNum;
                }

                public void setPersonNum(<span style="color: #007020">long</span> personNum) {
                    this<span style="color: #333333">.</span>personNum <span style="color: #333333">=</span> personNum;
                }

                public String getFirstName() {
                    <span style="color: #008800; font-weight: bold">return</span> firstName;
                }

                public void setFirstName(String firstName) {
                    this<span style="color: #333333">.</span>firstName <span style="color: #333333">=</span> firstName;
                }

                public String getLastName() {
                    <span style="color: #008800; font-weight: bold">return</span> lastName;
                }

                public void setLastName(String lastName) {
                    this<span style="color: #333333">.</span>lastName <span style="color: #333333">=</span> lastName;
                }

                public List<span style="color: #333333">&lt;</span>String<span style="color: #333333">&gt;</span> getPhoneNumbers() {
                    <span style="color: #008800; font-weight: bold">return</span> phoneNumbers;
                }

                public void setPhoneNumbers(List<span style="color: #333333">&lt;</span>String<span style="color: #333333">&gt;</span> phoneNumbers) {
                    this<span style="color: #333333">.</span>phoneNumbers <span style="color: #333333">=</span> phoneNumbers;
                }

            }
            </pre>
          </div>
        </div>
        <div style="width: 17%">
          <img
            src="../assets/illustrations/PersonClassDia.svg"
            style="width: 100%"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
