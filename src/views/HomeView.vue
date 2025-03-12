<script setup lang="ts"></script>

<template>
  <main id="main">
    <!-- Navigation section -->
    <section class="nav-section">
      <div class="nav-container">
        <a href="#" class="nav-item">Ferramentas de IA</a>
        <a href="#" class="nav-item">Documentação</a>
        <a href="#" class="nav-item">Colabore</a>
      </div>
    </section>

    <!-- Content container -->
    <div class="content-container">
      <!-- Chat section -->
      <section class="chat-section">
        <div class="chat-header">
          <h1>Drakunath AI</h1>
          <h2>Sua xxxxxxxx virtual</h2>
        </div>

        <div class="chat-gui">
          <div class="chat-contact">
            <img src="@/assets/date.png" alt="Drakunath profile" />
            <span>Drakunathy</span>
          </div>

          <div class="chat-content">
            <div class="chat-message">
              <img class="message-image" src="@/assets/date.png" alt="Drakunath avatar" />
              <p class="message-text">Estou esperando, cade você?</p>
            </div>
          </div>
          <div class="input-container">
            <input class="chat-input" type="text" placeholder="Converse com Nathalya" />
            <button class="chat-button">Enviar</button>
          </div>
        </div>
      </section>

      <!-- Info section -->
      <section class="info-section">
        <div class="info-header">
          <h1>Redes sociais</h1>
        </div>

        <div class="info-cards">
          <a href="#" class="card card-instagram">
            <i class="social-icon icon-instagram"></i>
            <span>Instagram</span>
          </a>
          <a href="#" class="card card-twitter">
            <i class="social-icon icon-twitter"></i>
            <span>Twitter</span>
          </a>
          <a href="#" class="card card-twitch">
            <i class="social-icon icon-twitch"></i>
            <span>Twitch</span>
          </a>
          <a href="#" class="card card-tiktok">
            <i class="social-icon icon-tiktok"></i>
            <span>Tiktok</span>
          </a>
          <a href="#" class="card card-discord">
            <i class="social-icon icon-discord"></i>
            <span>Comunidade no Discord</span>
          </a>
          <a href="#" class="card card-pinterest">
            <i class="social-icon icon-pinterest"></i>
            <span>Pinterest</span>
          </a>
        </div>
      </section>
    </div>
  </main>
</template>

<style scoped>
#main {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  border-radius: 12px;
  font-family: 'Poppins', sans-serif;
  padding: 1.5vh;
  background-color: #121212;
  min-height: 100vh;
  overflow: hidden;
}

/* Content container to hold chat and info sections */
.content-container {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  flex: 1;
}

/* Navigation Section Styles */
.nav-section {
  position: sticky;
  top: 0;
  z-index: 100;
  padding: 1.25rem;
  background: linear-gradient(135deg, #bd0171, #ff0090);
  border-radius: 12px;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
}

.nav-container {
  display: flex;
  justify-content: center;
  gap: 2rem;
  flex-wrap: wrap;
}

.nav-item {
  color: white;
  font-weight: 600;
  font-size: 1.2rem;
  text-decoration: none;
  padding: 0.75rem 1.5rem;
  border-radius: 8px;
  background-color: rgba(0, 0, 0, 0.3);
  transition: all 0.3s ease;
  letter-spacing: 0.5px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.2);
  text-align: center;
}

.nav-item:hover {
  background-color: rgba(0, 0, 0, 0.5);
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.3);
}

/* Chat Section Styles */
.chat-section {
  display: flex;
  flex-direction: column;
  padding: 1.25rem;
  background-color: rgba(20, 20, 20, 0.95);
  color: rgb(220, 220, 220);
  position: relative;
  background-image:
    linear-gradient(rgba(20, 20, 20, 0.85), rgba(20, 20, 20, 0.95)), url('@/assets/bg-pattern.png');
  background-size: cover;
  border: 2px solid black;
  border-radius: 12px;
}

.chat-header {
  text-align: center;
  margin-bottom: 1.5rem;
}

.chat-header h1 {
  line-height: 1.2;
  color: #ff0090;
  text-shadow: 0 0 15px #5f0096;
  font-size: 2.5rem;
  letter-spacing: 1px;
  font-weight: 800;
}

.chat-header h2 {
  line-height: 1.2;
  color: rgb(150, 150, 150);
  text-shadow: 0 0 10px #5f0096;
  font-size: 1.2rem;
  font-weight: 400;
  margin-top: 0.5rem;
}

.chat-gui {
  display: flex;
  flex-direction: column;
  border: 2px solid #ff0090;
  border-radius: 12px;
  box-shadow: 0 0 20px rgba(255, 0, 144, 0.3);
  flex: 1;
  width: 100%;
  overflow: hidden;
  height: 400px;
}

.chat-contact {
  display: flex;
  align-items: center;
  padding: 0.75rem 1rem;
  background: linear-gradient(to right, #bd0171, #ff0090);
  border-bottom: 1px solid #ff0090;
  border-radius: 10px 10px 0 0;
  cursor: pointer;
}

.chat-contact:hover {
  background: linear-gradient(to right, #ff0090, #bd0171);
}

.chat-contact img {
  width: 50px;
  height: 50px;
  border-radius: 40%;
  margin-right: 1rem;
  transition: all 0.3s;
  cursor: pointer;
  border: 2px solid rgba(255, 255, 255, 0.3);
}

.chat-contact img:hover {
  border-radius: 25%;
}

.chat-contact span {
  color: black;
  font-size: 1.5rem;
  font-weight: 600;
  letter-spacing: 0.5px;
}

.chat-content {
  flex: 1;
  display: flex;
  justify-content: flex-start;
  align-items: flex-start;
  padding: 1.5rem;
  overflow-y: auto;
  background-color: rgba(20, 20, 20, 0.9);
}

.chat-message {
  display: flex;
  align-items: flex-start;
  animation: fadeIn 0.5s ease-out;
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.message-image {
  width: 50px;
  height: 50px;
  border-radius: 40%;
  margin-right: 1rem;
  border: 2px solid rgba(255, 0, 144, 0.3);
}

.message-text {
  padding: 1rem 1.5rem;
  border-radius: 18px;
  background: linear-gradient(135deg, #bd0171, #ff0090);
  color: white;
  max-width: 80%;
  box-shadow: 0 3px 10px rgba(0, 0, 0, 0.2);
  font-size: 1rem;
  position: relative;
}

.message-text::after {
  content: '';
  position: absolute;
  left: -8px;
  top: 15px;
  width: 0;
  height: 0;
  border-top: 8px solid transparent;
  border-bottom: 8px solid transparent;
  border-right: 10px solid #bd0171;
}

.input-container {
  display: flex;
  background-color: rgba(20, 20, 20, 0.9);
  border-top: 1px solid #ff0090;
  border-radius: 0 0 10px 10px;
}

.chat-input {
  width: 100%;
  padding: 1rem 1.5rem;
  font-size: 1rem;
  border: none;
  border-top: 1px solid rgba(255, 0, 144, 0.5);
  background-color: rgba(20, 20, 20, 0.9);
  color: white;
  border-radius: 0 0 0 10px;
  outline: none;
  transition: background-color 0.3s;
}

.chat-input:focus {
  background-color: rgba(30, 30, 30, 0.95);
  box-shadow: 0 -2px 10px rgba(255, 0, 144, 0.2);
}

.chat-input::placeholder {
  color: rgba(255, 255, 255, 0.6);
}

.chat-button {
  background-color: #bd0171;
  padding: 1rem 1.5rem;
  color: white;
  font-size: 1rem;
  font-weight: 600;
  border: none;
  border-radius: 0 0 10px 0;
  cursor: pointer;
  transition: background-color 0.2s;
  color: black;
  font-weight: 400;
  width: 120px;
}

.chat-button:hover {
  background-color: #8b0054;
}

/* Info Section Styles */
.info-section {
  display: flex;
  flex-direction: column;
  padding: 1.25rem;
  background: linear-gradient(135deg, #bd0171, #ff0090);
  color: white;
  position: relative;
  border-radius: 12px;
}

.info-section::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-image: url('@/assets/pattern.png');
  background-size: 200px;
  opacity: 0.1;
  pointer-events: none;
  border-radius: 12px;
}

.info-header {
  text-align: center;
  margin-bottom: 1.5rem;
}

.info-header h1 {
  font-size: 2.2rem;
  font-weight: 700;
  color: white;
  text-shadow: 0 0px 7px rgba(0, 0, 0, 1);
  letter-spacing: 1px;
}

.info-cards {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1rem;
}

.card {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 1.25rem;
  background-color: rgba(0, 0, 0, 0.7);
  color: white;
  border-radius: 12px;
  font-weight: 600;
  font-size: 1.1rem;
  cursor: pointer;
  transition: all 0.3s ease;
  text-decoration: none;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
  position: relative;
  overflow: hidden;
  letter-spacing: 0.5px;
  border-inline: 8px solid #000;
}

.card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(45deg, rgba(255, 255, 255, 0.1), transparent);
  opacity: 0;
  transition: opacity 0.3s;
}

.card:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
}

.card:hover::before {
  opacity: 1;
}

.social-icon {
  margin-right: 10px;
  font-size: 1.3rem;
}

/* Media query for responsiveness */
@media (min-width: 1200px) {
  .content-container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1rem;
  }
}

@media (min-width: 768px) and (max-width: 1199px) {
  .info-cards {
    grid-template-columns: repeat(2, 1fr);
  }

  .chat-button {
    width: 100px;
  }

  .nav-container {
    gap: 1rem;
  }
}

@media (max-width: 767px) {
  .chat-section,
  .info-section {
    padding: 1rem;
  }

  .chat-header h1 {
    font-size: 1.8rem;
  }

  .info-header h1 {
    font-size: 1.6rem;
  }

  .info-cards {
    grid-template-columns: repeat(2, 1fr);
  }

  .chat-gui {
    height: 350px;
  }

  .chat-contact span {
    font-size: 1.2rem;
  }

  .chat-button {
    width: 80px;
    font-size: 0.9rem;
    padding: 1rem;
  }

  .nav-container {
    flex-direction: column;
    gap: 0.5rem;
  }

  .nav-item {
    width: 100%;
    font-size: 1rem;
    padding: 0.5rem 1rem;
  }
}

@media (max-width: 480px) {
  .chat-header h1 {
    font-size: 1.5rem;
  }

  .chat-header h2 {
    font-size: 1rem;
  }

  .chat-contact img {
    width: 40px;
    height: 40px;
  }

  .message-image {
    width: 40px;
    height: 40px;
  }

  .chat-gui {
    height: 300px;
  }

  .info-cards {
    grid-template-columns: 1fr;
  }
}
</style>
