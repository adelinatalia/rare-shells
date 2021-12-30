<template>
  <section class="info-container">
    <h2>6 of the most rare and beautiful shells</h2>
    <div class="info">
      <div class="info-txt">
        <p>
          With an estimated 120,000 species of shells (mollusks) worldwide,
          their appearance can vary greatly.
        </p>
        <br />
        <p>
          Shell jewelry has an incredibly ancient history, the oldest shell
          necklace dates back over 100,000 years and is made from the Swollen
          Nassa seashell.
        </p>
        <br />
        <p>
          Today, mollusks are still widely used in the jewelry trade,
          particularly mother of pearl and abalone shells thanks to their
          lustrous opalescent finish.
        </p>
      </div>
      <div class="info-img">
        <img src="../assets/images/shell-blue.png" alt="shell" width="300" />
      </div>
    </div>
  </section>
</template>

<style>
.info-container {
  width: 80vw;
  margin: 0 auto;
  padding: 2rem;
  background-color: #fff;
  border-radius: 5px;
  position: relative;
  top: 3.5rem;
}

.info-container h2 {
  font-size: 1.8em;
  padding: 1.5rem 0;
  color: var(--primary);
}

.info {
  display: flex;
}

.info-txt {
  margin-top: 1.5rem;
  padding-left: 3rem;
  text-align: left;
  line-height: 1.5;
}

.info-img {
  margin: 0.5rem 1rem 1rem 1rem;
}

.info-img img {
  width: 100%;
}

/* smart phone */
@media only screen and (max-width: 550px) {
  .info {
    flex-direction: column;
  }

  .info-img {
    order: 1;
    margin: 0;
  }

  .info-txt {
    order: 2;
    padding: 1rem;
    padding-top: 0;
  }

  .info-container h2 {
    font-size: 1.5em;
  }
}
</style>