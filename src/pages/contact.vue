<template>
  <section id="hire">
    <h1><u>Contact Us</u></h1>

    <form>
      <div class="field name-box">
        <input type="text" id="name" placeholder="Who Are You?" />
        <label for="name">Name</label>
        <span class="ss-icon">check</span>
      </div>

      <div class="field email-box">
        <input type="text" id="email" placeholder="name@email.com" />
        <label for="email">Email</label>
        <span class="ss-icon">check</span>
      </div>

      <div class="field msg-box">
        <textarea
          id="msg"
          rows="10"
          placeholder="Your message goes here..."
        ></textarea>
        <label for="msg">Message</label>
        <span class="ss-icon">check</span>
      </div>

      <input class="button" type="submit" value="Send" />
    </form>
  </section>
</template>
