<script setup lang="ts"></script>

<template>
  <main id="main">
    <!-- Chat section -->
    <section class="chat-section">
      <div class="chat-header">
        <h1>Drakunath AI</h1>
        <h2>Sua xxxxxxxx virtual</h2>
      </div>

      <div class="chat-gui">
        <div class="chat-contact">
          <img src="@/assets/date.png" alt="Drakunath profile" />
          <span>Drakunath</span>
        </div>

        <div class="chat-content">
          <div class="chat-message">
            <img class="message-image" src="@/assets/date.png" alt="Drakunath avatar" />
            <p class="message-text">Drakunathy está digitando..</p>
          </div>
        </div>

        <input class="chat-input" type="text" placeholder="Comece a conversar" />
      </div>
    </section>

    <!-- Info section -->
    <section class="info-section">
      <div class="info-header">
        <h1>Redes sociais</h1>
      </div>

      <div class="info-cards">
        <div class="card card-1">Instagram</div>
        <div class="card card-2">Twitter</div>
        <div class="card card-3">Twitch</div>
        <div class="card card-4">Tiktok</div>
        <div class="card card-4">Comunidade no Discord</div>
        <div class="card card-4">Pinterest</div>
      </div>
    </section>
  </main>
</template>

<style scoped>
#main {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 0.5rem;
  border-radius: 12px;
  overflow: hidden;
  flex: 1;
}

/* Chat Section Styles */
.chat-section {
  display: flex;
  flex-direction: column;
  padding: 2rem;
  background-color: rgba(20, 20, 20, 0.95);
  color: rgb(220, 220, 220);
}

.chat-header {
  text-align: center;
  margin-bottom: 1.5rem;
}

.chat-header h1 {
  line-height: 1.2;
  color: #bd0171;
  text-shadow: 0 0 10px #a200ff8f;
}

.chat-header h2 {
  line-height: 1.2;
  color: rgb(120, 120, 120);
  text-shadow: 0 0 10px #a200ff8f;
}

.chat-gui {
  display: flex;
  flex-direction: column;
  border: 2px solid black;
  box-shadow: 1px 1px 10px 0px black;
  flex: 1;
  width: 100%;
}

.chat-contact {
  display: flex;
  align-items: center;
  padding: 0.5rem;
  background-color: rgba(189, 1, 113, 0.75);
  border-bottom: 1px solid #bd0171;
}

.chat-contact img {
  width: 50px;
  height: 50px;
  border-radius: 40%;
  margin-right: 1rem;
  transition: all 0.2s;
  cursor: pointer;
}

.chat-contact img:hover {
  border-radius: 35%;
}

.chat-contact span {
  color: black;
  font-size: 1.5rem;
  font-weight: 500;
}

.chat-contact:hover span {
}

.chat-content {
  flex: 1;
  display: flex;
  justify-content: flex-start;
  align-items: flex-start;
  padding: 1rem;
  overflow-y: auto;
}

.chat-message {
  display: flex;
  align-items: flex-start;
}

.message-image {
  width: 50px;
  height: 50px;
  border-radius: 40%;
  margin-right: 1rem;
}

.message-text {
  padding: 1rem;
  border-radius: 1rem;
  background-color: #bd0171;
  color: white;
  max-width: 80%;
}

.chat-input {
  width: 100%;
  padding: 1rem;
  font-size: 1rem;
  border: none;
  border-top: 1px solid #bd0171;
  background-color: rgba(189, 1, 114, 0.75);
  color: white;
}

.chat-input::placeholder {
  color: rgb(20, 20, 20);
}

/* Info Section Styles */
.info-section {
  display: flex;
  flex-direction: column;
  padding: 2rem;
  background-color: rgba(189, 1, 113, 0.75);
  color: black;
}

.info-header {
  text-align: center;
  margin-bottom: 2rem;
}

.info-cards {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  flex: 1;
}

.card {
  padding: 1.5rem;
  background-color: rgba(0, 0, 0, 0.8);
  color: white;
  border-radius: 8px;
  font-weight: bold;
  cursor: pointer;
  transition:
    transform 0.2s,
    box-shadow 0.2s;
  text-align: center;
}

.card:hover {
  transform: translateY(-3px);
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
}
</style>
