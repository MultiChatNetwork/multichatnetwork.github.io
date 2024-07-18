<template>
  <MainLayout>
    <main class="row p-0 m-0">
      <section class="stars-section col-md-4 p-0 m-0">
        <div class="stars">
          <div class="animation stars-small" />
          <div class="animation stars-large" />
        </div>
        <h1 class="stars-section-text">MultiChat</h1>
      </section>

      <section class="col-md-8 p-0 m-0">
        <header class="multichat-header px-4 my-4 px-md-5 my-md-5">
          <nav class="multichat-nav">
            <ul class="multichat-list">
              <li class="multichat-list-item">
                <h4 class="mv-primary-headline headline bg-primary">MultiChat.network</h4>
              </li>
            </ul>
            <ul class="multichat-list d-flex align-items-center justify-content-end gap-3">
              <li class="multichat-list-item">
                <a class="multichat-list-link" href="https://help.multividas.com/multichat/security" target="_blank">Security</a>
              </li>
              <li class="multichat-list-item">
                <a class="multichat-list-link" href="https://developers.multividas.com/products/multichat/getting-started" target="_blank">Developers</a>
              </li>
            </ul>
          </nav>
        </header>

        <section class="multichat-content px-4 px-md-5">
            <ul class="multichat-content-list mb-4 mb-md-5">
              <li class="multichat-content-item">
                <span
                  role="button"
                  class="fw-bold text-primary text-decoration-underline"
                  @click="handleRedirect()"
                >
                  @soulaimaneyahya
                </span>
                <span>CEO-Founder | Software Engineer at MultiChat</span>
              </li>
              <li class="multichat-content-item">
                Multichat is a messaging app with focus on security & user
                experience
              </li>
              <li class="multichat-content-item">
                Messages are end-to-end encrypted. No one outside of chat
                inbox, not even MultiChat, can read or listen to messages.
              </li>
              <li class="multichat-content-item">
                Built-in layers of security give you the peace of mind to
                focus on connecting with family and friends.
              </li>
            </ul>

            <div class="multichat-footer mb-4 mb-md-0">
              <button class="btn btn-primary rounded-3" @click="handleRedirectMultividas()" >
                Login with Multividas
              </button>

              <p class="appreciation-text">
                Thank you, the MultiChat Team
              </p>
            </div>
        </section>
      </section>
    </main>
  </MainLayout>
</template>

<script>
export default {
  metaInfo: {
    title: "Home Page",
  },
  methods: {
    handleRedirect() {
      return window.open("https://soulaimaneyahya.com/", "_blank");
    },
    handleRedirectMultividas() {
      return window.open("https://multividas.com/?ref=login&source=multichat.network", "_blank");
    }
  },
};
</script>
