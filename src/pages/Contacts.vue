<template>
    <footer class="site-footer" id="contacts">
      <div class="container">
        <div class="row">
          <div class="col-md-4">
            <h4>Link utili</h4>
            <ul>
              <li><a href="#home">Home</a></li>
              <li><a href="#about">Chi sono</a></li>
              <li><a href="#services">Servizi</a></li>
              <li><a href="#contact">Contattaci</a></li>
            </ul>
          </div>
          <div class="col-md-4">
            <h4>Contatti</h4>
            <p>Indirizzo: Via Example, 18012, Bordighera</p>
            <p>Telefono: +39 327 9171289</p>
            <p>Email: info@andreacassini.com</p>
          </div>
          <div class="col-md-4">
            <h4>Richiesta informazioni</h4>
            <form @submit.prevent="submitRequest">
              <div class="form-group">
                <label for="name">Nome:</label>
                <input type="text" id="name" v-model="requestName" required>
              </div>
              <div class="form-group">
                <label for="email">Email:</label>
                <input type="email" id="email" v-model="requestEmail" required>
              </div>
              <div class="form-group">
                <label for="message">Messaggio:</label>
                <textarea id="message" v-model="requestMessage" required></textarea>
              </div>
              <button type="submit">Invia richiesta</button>
            </form>
          </div>
        </div>
      </div>
    </footer>
  </template>
  
  <script>
  export default {
    data() {
      return {
        requestName: '',
        requestEmail: '',
        requestMessage: '',
      };
    },
    methods: {
      submitRequest() {
        // Esegui azioni per inviare la richiesta di informazioni qui (ad esempio, una richiesta API)
        console.log('Nome:', this.requestName);
        console.log('Email:', this.requestEmail);
        console.log('Messaggio:', this.requestMessage);
        // Pulisci i campi del modulo
        this.requestName = '';
        this.requestEmail = '';
        this.requestMessage = '';
      },
    },
  };
  </script>
  
  <style scoped>
  .site-footer {
    background-color: #333;
    color: #fff;
    padding: 40px 0;
  }
  
  .site-footer h4 {
    color: #fff;
  }
  
  .site-footer ul {
    list-style: none;
    padding: 0;
  }
  
  .site-footer ul li {
    margin-bottom: 10px;
  }
  
  .site-footer a {
    color: #fff;
    text-decoration: none;
  }
  
  .site-footer a:hover {
    text-decoration: underline;
  }
  
  .form-group {
    margin-bottom: 10px;
  }
  
  label {
    display: block;
    font-weight: bold;
  }
  
  input,
  textarea {
    width: 100%;
    padding: 5px; /* Ridotto il padding */
    border: 1px solid #ccc;
    border-radius: 5px;
  }
  
  button {
    background-color: #007bff;
    color: #fff;
    padding: 5px 10px; /* Ridotto il padding */
    border: none;
    border-radius: 5px;
    cursor: pointer;
  }
  </style>
  