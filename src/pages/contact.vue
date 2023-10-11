<template>
  <section class="mb-4">
    <!--Section heading-->
    <h2 class="h1-responsive font-weight-bold text-center my-4">Contact</h2>
    <!--Section description-->
    <p class="text-center w-responsive mx-auto mb-5">
      Vous avez des questions ? Contactez-moi, je me ferais un plaisir de vous
      repondre.
    </p>

    <div class="row contactform">
      <!--Grid column-->
      <div class="col-md-9 mb-md-0 mb-5">
        <form
          id="contact-form"
          name="contact-form"
          action="mail.php"
          method="POST"
        >
          <!--Grid row-->
          <div class="row contactform">
            <!--Grid column-->
            <div class="col-md-6">
              <div class="md-form mb-0">
                <input
                  type="text"
                  id="name"
                  name="name"
                  placeholder="Votre Nom"
                  class="form-control"
                />
              </div>
            </div>
            <!--Grid column-->

            <!--Grid column-->
            <div class="col-md-6">
              <div class="md-form mb-0">
                <input
                  type="text"
                  id="email"
                  name="email"
                  class="form-control"
                  placeholder="Votre email"
                />
              </div>
            </div>
            <!--Grid column-->
          </div>
          <!--Grid row-->

          <!--Grid row-->
          <div class="row contactform">
            <div class="col-md-12">
              <div class="md-form mb-0">
                <input
                  type="text"
                  id="subject"
                  name="subject"
                  class="form-control"
                  placeholder="Votre sujet"
                />
              </div>
            </div>
          </div>
          <!--Grid row-->

          <!--Grid row-->
          <div class="row contactform">
            <!--Grid column-->
            <div class="col-md-12">
              <div class="md-form">
                <textarea
                  type="text"
                  id="message"
                  name="message"
                  rows="2"
                  class="form-control md-textarea"
                  placeholder="Dites m'en plus"
                ></textarea>
              </div>
            </div>
          </div>
          <!--Grid row-->
        </form>

        <div class="text-center text-md-left" style="margin-top: 1rem">
          <a
            class="btn btn-primary"
            onclick="document.getElementById('contact-form').submit();"
            >Send</a
          >
        </div>
        <div class="status"></div>
      </div>
      <!--Grid column-->

      <!--Grid column-->
      <div class="col-md-3 text-center">
        <ul class="list-unstyled mb-0">
          <li>
            <i class="fas fa-map-marker-alt fa-2x"></i>
            <p>Bruxelles, Belgique</p>
          </li>

          <li>
            <i class="fas fa-phone mt-4 fa-2x"></i>
            <p>+32 494 46 46 38</p>
          </li>

          <li>
            <i class="fas fa-envelope mt-4 fa-2x"></i>
            <p>GabrielEtolo0@gmail.com</p>
          </li>
        </ul>
      </div>
      <!--Grid column-->
    </div>
  </section>
</template>
