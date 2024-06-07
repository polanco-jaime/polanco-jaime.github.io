---
layout: about
permalink: /
title: "<strong>Jaime</strong> Polanco-Jimenez"
order: 1
description: >
  <span style="font-size: 1.2em;">🚀 Exciting News: I will be on the Job Market in 2025/2026!</span>
  <br/>
  Interested in Development Economics, Economics of Education, Natural Resource Economics, and being an enthusiastic data scientist.
  <br/>
  <blockquote2 class="warning" id="mymotto" title="Motto"><h5>'Nothing is built on stone, all is built on sand; but we must build as if the sand were stone.'<br/> – Jorge Luis Borges</h5></blockquote2>
profile:
  align: right
  image: prof_pic.jpg
news: true
social: true
---

<template>
  <!-- Navigation -->
  <nav class="bg-white shadow-lg h-25">
    <div class="container mx-auto flex justify-between items-center">
      <a href="#"></a>
    </div>
  </nav>

  <!-- Hero Section -->
  <div class="bg-gradient-to-r from-red-500 to-orange-600 text-white py-20">
    <div class="container mx-auto text-center">
      <h1 class="text-4xl md:text-6xl font-bold">
        Centro de contacto de Riopaila
      </h1>
      <p class="text-lg mt-4">
        Acá podrás comunicarte con nosotros para resolver tus dudas o
        inquietudes de una manera rápida y eficiente.
      </p>
      <a
        href="#chat"
        class="
          mt-8 px-6 py-4
          inline-block
          bg-white text-orange-500
          font-bold
          rounded-lg
          shadow-lg
        "
      >
        Contáctanos
      </a>
    </div>
  </div>

  <div id="chat" class="w-full px-1 h-screen bg-gray-100">
    <div v-if="loading" role="status" class="pt-5 px-5 w-full animate-pulse">
      <div class="h-5 bg-gray-200 rounded-full w-48 float-right"></div>
      <div class="h-5 bg-gray-200 rounded-full w-48 my-2"></div>
      <div class="h-20 bg-gray-200 rounded-full w-1/2 my-2"></div>
      <div class="h-10 bg-gray-200 rounded-full w-1/2 my-2"></div>
      <div class="h-5 bg-gray-200 rounded-full w-1/3 my-2 float-right"></div>
      <div class="h-10 bg-gray-200 rounded-full w-1/3 my-2"></div>
      <div class="h-10 bg-gray-200 rounded-full w-1/4 my-2"></div>
      <div class="h-10 bg-gray-200 rounded-full w-1/4 my-2"></div>
      <div class="h-10 bg-gray-200 rounded-full w-1/3 my-2"></div>
      <div class="h-10 bg-gray-200 rounded-full w-1/3 my-2 float-right"></div>
    </div>
  </div>

  <!-- Features Section -->
  <div class="container mx-auto py-20">
    <div class="flex flex-wrap -mx-4">
      <div class="w-full md:w-1/3 px-4 mb-8">
        <div class="bg-white rounded-lg p-6 shadow-lg">
          <h2 class="text-xl font-bold mb-4">Usamos IA</h2>
          <p class="text-gray-700">
            Usamos inteligencia artificial para responder tus preguntas
          </p>
        </div>
      </div>
      <div class="w-full md:w-1/3 px-4 mb-8">
        <div class="bg-white rounded-lg p-6 shadow-lg">
          <h2 class="text-xl font-bold mb-4">Comunicación rápida</h2>
          <p class="text-gray-700">
            Te responderemos en el menor tiempo posible
          </p>
        </div>
      </div>
      <div class="w-full md:w-1/3 px-4 mb-8">
        <div class="bg-white rounded-lg p-6 shadow-lg">
          <h2 class="text-xl font-bold mb-4">Soporte 24/7</h2>
          <p class="text-gray-700">
            Estamos disponibles las 24 horas del día, los 7 días de la semana
          </p>
        </div>
      </div>
    </div>
  </div>

  <!-- Footer Section -->
  <footer class="bg-gray-800 text-white py-10">
    <div class="container mx-auto text-center">
      <p>&copy; 2024 Riopaila. Todos los derechos reservados.</p>
    </div>
  </footer>
</template>

<script setup lang="ts">
import { onMounted, ref } from 'vue';

const loading = ref(false);

const openDialogFlow = () => {
  const chatEl = document.getElementById('chat') as HTMLElement;

  const dfMessenger = document.createElement('df-messenger');
  dfMessenger.setAttribute('location', 'us-central1');
  dfMessenger.setAttribute('project-id', 'novyye-produkty');
  dfMessenger.setAttribute('agent-id', 'dd6837ef-da45-44f4-b222-ccfaff6ade5b');
  dfMessenger.setAttribute('language-code', 'en');
  dfMessenger.setAttribute('max-query-length', '-1');

  const dfMessengerChat = document.createElement('df-messenger-chat');
  dfMessengerChat.setAttribute('chat-title', 'Jaime Bot');

  dfMessenger.appendChild(dfMessengerChat);

  // set dialogflow chat to visible
  chatEl?.appendChild(dfMessenger);

  console.log(chatEl);
};

onMounted(async () => {
  openDialogFlow();
  loading.value = true;
  // random number between 1 and 5
  const randomNumber = Math.floor(Math.random() * 5) + 1;
  // eslint-disable-next-line no-promise-executor-return
  await new Promise((r) => setTimeout(r, randomNumber * 1000));
  loading.value = false;
});
</script>

<style lang="scss">
@import "https://www.gstatic.com/dialogflow-console/fast/df-messenger/prod/v1/themes/df-messenger-default.css";
html {
  scroll-behavior: smooth;
}

df-messenger {
  --df-messenger-font-color: #ec930c;
  --df-messenger-font-color: #333333;
  --df-messenger-chat-background: #ffffff;
  --df-messenger-message-user-background: rgb(243 244 246);
  --df-messenger-message-bot-background: #fef3e8;
}
</style>
