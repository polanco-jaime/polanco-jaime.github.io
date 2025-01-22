---
layout: category-page
title: Article Category
category: article
---



## Chat with our Agent

<p>Interact with our chatbot below:</p>

<div style="position: relative; height: 500px; width: 100%;">
  <df-messenger
      location="europe-west1"
      project-id="groep2-belastingsystemen"
      agent-id="9533f5bc-195d-42de-9b0f-6b9ae4309884"
      language-code="nl"
      chat-title="Agent Name" <!-- Update dialog title -->
  ></df-messenger>
</div>

<script src="https://www.gstatic.com/dialogflow-console/fast/df-messenger/prod/v1/df-messenger.js"></script>

<script>
  // Event listener to navigate to the first suggested URL.
  document.addEventListener('df-url-suggested', (event) => {
    if (Array.isArray(event.detail.suggestedUrls) &&
      event.detail.suggestedUrls.length) {
      window.location.href = event.detail.suggestedUrls[0];
    }
  });
</script>