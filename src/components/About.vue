<template>
  <div id="app">
    <main class="content">
      <div class="box-container">
        <h1>Avis de passage n°...</h1>
        <div class="container">
          <p>Bonjour, M./Mme,</p>
          <p>Nous allons intervenir aujourd’hui à partir de *DATE ET HEURE DE DEBUT* jusqu’à *DATE ET HEURE DE FIN* au *RUE/ADRESSE* pour l’intervention *TITLE* prévue en ce jour.</p>
        </div>

        <div class="after-container">
          <p>Vous avez besoin d’informations complémentaires ou vous souhaitez reporter l’intervention ? Contactez-nous dès maintenant en répondant à notre email ou téléphone.</p>
          <router-link to="home"><button class="button">Retour</button></router-link>
        </div>
      </div>
    </main>
  </div>
</template>

<style scoped>
h1 {
  font-family: kanit;
  text-align: center;
  padding: 20px;
  color: #000000;
}

.button {
  font-family: kanit;
  color: #ffffff;
  background-color: #55ab41;
  margin: 5px;
  padding: 10px;
  width: 200px;
  border-color: #ffffff;
  border-style: none;
  border-radius: 10px;
}

.center-button {
  display: flex;
  justify-content: center;
}

.button:last-child {
  margin-left: auto;
}

.content {
  align-items: center;
  width: auto;
  background: white;
  height: 100vh;
}

.box-container {
  text-align: center;
  background-color: #ffffff;
  padding: 20px;
  margin: 50px;
  border: 2px solid #ccc;
  border-radius: 10px;
  box-shadow: 0 4px 4px rgba(0, 0, 0, 0.1);
  overflow: hidden; 
}

@media (max-width: 768px) {
  .box-container {
    margin: 20px;
    padding: 10px;
  }

  .button {
    width: 100%;
  }
}
</style>
