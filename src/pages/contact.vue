<template>
  <section class="mb-4">
    <!-- Section heading -->
    <h2 class="h1-responsive font-weight-bold text-center my-4">Contact</h2>
    <!-- Section description -->
    <p class="text-center w-responsive mx-auto mb-5">
      Vous avez des questions ? Contactez-moi, je me ferais un plaisir de vous
      répondre.
    </p>

    <div class="row contactform">
      <!-- Grid column -->
      <div class="col-md-9 mb-md-0 mb-5">
        <form @submit.prevent="submitForm">
          <!-- Grid row -->
          <div class="row contactform">
            <!-- Grid column -->
            <div class="col-md-6">
              <div class="md-form mb-0">
                <input
                  v-model="formData.name"
                  type="text"
                  placeholder="Votre Nom"
                  class="form-control"
                />
              </div>
            </div>
            <!-- Grid column -->

            <!-- Grid column -->
            <div class="col-md-6">
              <div class="md-form mb-0">
                <input
                  v-model="formData.email"
                  type="text"
                  class="form-control"
                  placeholder="Votre email"
                />
              </div>
            </div>
            <!-- Grid column -->
          </div>
          <!-- Grid row -->

          <!-- Grid row -->
          <div class="row contactform">
            <div class="col-md-12">
              <div class="md-form mb-0">
                <input
                  v-model="formData.subject"
                  type="text"
                  class="form-control"
                  placeholder="Votre sujet"
                />
              </div>
            </div>
          </div>
          <!-- Grid row -->

          <!-- Grid row -->
          <div class="row contactform">
            <!-- Grid column -->
            <div class="col-md-12">
              <div class="md-form">
                <textarea
                  v-model="formData.message"
                  rows="2"
                  class="form-control md-textarea"
                  placeholder="Dites m'en plus"
                ></textarea>
              </div>
            </div>
          </div>
          <!-- Grid row -->

          <div class="text-center text-md-left" style="margin-top: 1rem">
            <button type="submit" class="btn btn-primary">Envoyer</button>
          </div>
          <div class="status">{{ formStatus }}</div>
        </form>
      </div>
      <!-- Grid column -->

      <!-- Grid column -->
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
      <!-- Grid column -->
    </div>
  </section>
</template>
<script>
import axios from "axios";
export default {
  data() {
    return {
      formData: {
        name: "",
        email: "",
        subject: "",
        message: "",
      },
      formStatus: "",
    };
  },
  methods: {
    submitForm() {
      const { name, email, subject, message } = this.formData;
      if (name && email && subject && message) {
        // You can send the form data to your server using Axios or any other HTTP library.
        // Example using Axios:
        axios
          .post("your_server_endpoint", this.formData)
          .then((response) => {
            this.formStatus = "Email sent!";
          })
          .catch((error) => {
            this.formStatus = "Error sending email.";
          });

        // For demonstration, let's assume the form is sent successfully.
      } else {
        this.formStatus = "Veuillez remplir le formulaire";
      }
    },
  },
};
</script>
