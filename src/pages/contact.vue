<template>
  <section class="mb-4">
    <!-- Section heading -->

    <form>
      <div class="form">
        <div class="form-txt">
          <h1>Contact</h1>
          <span>
            Vous avez des questions ? <br />Contactez-moi, je me ferais un
            plaisir de vous répondre.</span
          >
          <h3>Belgique</h3>
          <p>Auderghem,Bruxelles<br />+324 94 46 46 38</p>
        </div>
        <div class="form-details">
          <input type="text" name="name" id="nom" placeholder="Nom" required />
          <input
            type="email"
            name="email"
            id="email"
            placeholder="Email"
            required
          />
          <textarea
            name="message"
            id="message"
            cols="52"
            rows="7"
            placeholder="Message"
            required
          ></textarea>
          <button>SEND MESSAGE</button>
        </div>
      </div>
    </form>
  </section>
</template>
