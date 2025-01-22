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

{: .text-justify}
# About Me
I am Jaime Polanco-Jiménez, a PhD student in Economics at [Leuven Economics of Education Research](https://research.kuleuven.be/portal/en/project/3H240489);  [Katholieke Universiteit Leuven](https://www.kuleuven.be/english/), Belgium and  Department of Economics at [Pontificia Universidad Javeriana](https://www.javeriana.edu.co/) 
 
 
{: .text-justify}


## Research Focus


My passion lies in applying rigorous economic analysis to address issues related to human capital accumulation, economics of education, and development economics. Specifically, my current research focuses on analyzing how AI can support the learning of students facing teacher shortage, Also the gender composition, the intervention on infrastructure, the artificial intelligence, the oil industry's influence on educational outcomes as measures of academic performance and human capital accumulation, with a particular emphasis on developing countries.   I conduct my research dissertation under the expert supervision of Professor [Gloria Bernal](https://cea.javeriana.edu.co/w/facultad-de-cea-profesores-econom%C3%8Da-17?redirect=%2Fprofesores), and Professor [Kristof De Witte](https://www.kuleuven.be/wieiswie/en/person/00049626).
{: .text-justify}



 

## Chat Bot

The Bibliographic Query Chatbot (BQC) in Economics is my own creation, designed as an essential tool for those who want to stay updated on the latest research and trends in the field of economics. Its capability to perform detailed queries and deliver precise analyses makes it a valuable resource for academics, researchers, and students alike.
{: .text-justify}

<div id="chat" class="w-full px-1 h-screen">
  <df-messenger
    location="us-central1"
    project-id="novyye-produkty"
    agent-id="dd6837ef-da45-44f4-b222-ccfaff6ade5b"
    language-code="en">
    <df-messenger-chat
    chat-title="Jaime Bot">
    </df-messenger-chat>
  </df-messenger>
</div>
 

<script src="https://www.gstatic.com/dialogflow-console/fast/df-messenger/prod/v1/df-messenger.js"></script>

<style>
  df-messenger {
    --df-messenger-bot-message: #004aad; /* Bot message background color - dark blue */
    --df-messenger-button-titlebar-color: #b76e2a; /* Title bar button color */
    --df-messenger-chat-background-color: #ffffff; /* Chat background color - pure white */
    --df-messenger-font-color: #000000; /* Font color for messages - black for high contrast */
    --df-messenger-send-icon: #fca103; /* Send icon color */
    --df-messenger-user-message: #005c2e; /* User message background color - dark green */
  }

  /* Ensure the custom properties are applied to the correct elements */
  df-messenger .chat-wrapper[opened] df-messenger-chat .message-list .message.user {
    background-color: var(--df-messenger-user-message);
  }

  df-messenger .chat-wrapper[opened] df-messenger-chat .message-list .message.bot {
    background-color: var(--df-messenger-bot-message);
  }

  df-messenger .chat-wrapper[opened] df-messenger-chat {
    background-color: var(--df-messenger-chat-background-color);
  }

  df-messenger .chat-wrapper[opened] df-messenger-chat .message-list .message {
    color: var(--df-messenger-font-color);
  }

  df-messenger .chat-wrapper[opened] df-messenger-titlebar {
    background-color: var(--df-messenger-button-titlebar-color);
  }

  df-messenger .chat-wrapper[opened] df-messenger-input {
    color: var(--df-messenger-font-color);
  }

  df-messenger .chat-wrapper[opened] df-messenger-send-icon {
    fill: var(--df-messenger-send-icon);
  }

  .df-messenger-message {
    font-family: Arial, sans-serif; /* Specify a fallback font */
    font-size: 18px; /* Increase font size for better readability */
    line-height: 1.5; /* Set line spacing */
    padding: 14px; /* Add padding for better spacing */
    margin: 10px 0; /* Add margins for better spacing between messages */
    color: var(--df-messenger-font-color); /* Apply the font color variable */
  }
  .w-full {
    width: 95%;
  }

  .px-1 {
    padding: 1.0rem, 0px;
  }

  .h-screen {
    height: 60vh;
  }
 
</style>  

<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-EHXV39ZW0B"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-EHXV39ZW0B');
</script>
 



 ## Chatbot 2


## Chat
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <meta http-equiv="Cache-Control" content="no-cache, no-store, must-revalidate" />
  <meta http-equiv="Pragma" content="no-cache" />
  <meta http-equiv="Expires" content="0" />
  <title>My chat</title>
  <style>
    df-messenger {
      /*
       * Customize as required. df-messenger will fill the
       * space that is provided.
      */
      position: absolute;
      right: 0;
      top: 0;
      bottom: 0;
      width: 320px;
    }
  </style>
  <script src="https://www.gstatic.com/dialogflow-console/fast/df-messenger/prod/v1/df-messenger.js"></script>
</head>
<body>
<df-messenger
    location="europe-west1"
    project-id="groep2-belastingsystemen"
    agent-id="9533f5bc-195d-42de-9b0f-6b9ae4309884"
    language-code="nl"
>
  <df-messenger-chat
      chat-title="Agent Name" <!-- TODO: update dialog title as needed -->
  ></df-messenger-chat>
</df-messenger>

<script>
  // An example of handling events: Navigate to the first suggested URL.
  document.addEventListener('df-url-suggested', (event) => {
    if (Array.isArray(event.detail.suggestedUrls) &&
      event.detail.suggestedUrls.length) {
      window.location.href = event.detail.suggestedUrls[0];
  }
});
</script>
</body>
</html>