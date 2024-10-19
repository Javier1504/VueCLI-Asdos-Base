<template>
  <div id="app">
    <div class="header">
      <img alt="Logo ITS" src="./assets/hmtc.jpg" class="logo">
    </div>
    <HelloWorld msg="saya warga c-25"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
/* Background dengan warna gradient yang lebih lembut */
body {
  background: linear-gradient(to right, #f5f7fa, #c3cfe2); /* Warna gradient soft blue */
  margin: 0;
  font-family: 'Poppins', Avenir, Helvetica, Arial, sans-serif;
  color: #333; /* Warna teks yang lebih netral */
}

/* Styling untuk aplikasi */
#app {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  text-align: center;
  padding: 20px;
}

/* Gaya pada logo */
.logo {
  width: 250px; /* Memperbesar ukuran logo */
  height: auto; /* Menjaga rasio aspek */
  border-radius: 15px; /* Rounded corners untuk logo */
  box-shadow: 0px 5px 15px rgba(0, 0, 0, 0.1); /* Bayangan halus */
  transition: transform 0.3s ease, box-shadow 0.3s ease; /* Animasi halus saat hover */
}

/* Efek hover pada logo */
.logo:hover {
  transform: scale(1.05); /* Membesar sedikit saat di-hover */
  box-shadow: 0px 10px 30px rgba(0, 0, 0, 0.2); /* Efek bayangan saat hover */
}

/* Styling untuk teks */
h1 {
  font-size: 2.5rem;
  margin-top: 20px;
  text-shadow: 1px 2px 4px rgba(0, 0, 0, 0.2); /* Bayangan halus pada teks */
  color: #333; /* Warna teks yang lebih netral */
}

/* Card styling untuk komponen HelloWorld */
.hello {
  background-color: #ffffff;
  border-radius: 15px;
  padding: 20px;
  box-shadow: 0px 5px 15px rgba(0, 0, 0, 0.1); /* Bayangan halus pada card */
  margin-top: 20px;
  max-width: 600px;
  transition: transform 0.3s ease, box-shadow 0.3s ease; /* Transisi halus */
}

.hello:hover {
  transform: scale(1.02); /* Efek hover halus */
  box-shadow: 0px 10px 30px rgba(0, 0, 0, 0.15); /* Bayangan saat hover */
}

/* Styling untuk paragraf */
p {
  font-size: 1.2rem;
  color: #666; /* Warna teks yang lebih lembut */
  line-height: 1.6;
}
</style>
