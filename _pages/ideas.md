---
layout: page
title: Interests
permalink: /ideas/
description: Past and future projects
order: 5
---


## Bot 2
ajhsdkjahs kjahsdjkahsd kjhasdj

<link rel="stylesheet" href="https://www.gstatic.com/dialogflow-console/fast/df-messenger/prod/v1/themes/df-messenger-default.css">
<script src="https://www.gstatic.com/dialogflow-console/fast/df-messenger/prod/v1/df-messenger.js"></script>
<df-messenger
  location="us-central1"
  project-id="servi-modelos-ia-dev"
  agent-id="d408e253-3124-496d-8c92-cad2225af0f3"
  language-code="en"
  max-query-length="-1">
  <df-messenger-chat
   chat-title="ADSMOVIL_2">
  </df-messenger-chat>
</df-messenger>
<style>
  df-messenger {
    z-index: 999;
    position: fixed;
    --df-messenger-font-color: #000;
    --df-messenger-font-family: Google Sans;
    --df-messenger-chat-background: #f3f6fc;
    --df-messenger-message-user-background: #d3e3fd;
    --df-messenger-message-bot-background: #fff;
    bottom: 0;
    right: 0;
    top: 0;
    width: 350px;
  }
</style>

<!--Tags generator-->
{% assign all_tags = '' | split: ',' %}

 {% for post in site.categories.idea %}
    {% for tags in post.tags %}
        {% for tag in tags %}
            {% assign all_tags = all_tags | push: tag %}
        {% endfor %}
    {% endfor %}
{% endfor %}

{% assign all_tags = all_tags | sort %}
{% assign all_tags = all_tags | uniq %}


<!--TagCloud-->
<center> <br><br>
{% include tagcloud.html %}
</center>


