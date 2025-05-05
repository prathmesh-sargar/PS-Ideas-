# 🤖 Create Your Own Custom Chatbot Using Botpress

This guide helps you create and embed your very own chatbot using [Botpress](https://botpress.com/) — a powerful no-code platform for building AI chatbots. You only need basic HTML knowledge to follow along!

---

## 🚀 What is Botpress?

Botpress is a free, user-friendly chatbot builder that allows you to create, customize, and manage AI bots easily through a visual interface. No complex coding required!

---

## ✅ Step-by-Step Guide

### 1. Sign up on Botpress
- Go to [https://botpress.com/](https://botpress.com/)
- Create a free account or log in

---

### 2. Create Your Chatbot
- After login, click on **"Create Bot"**
- Choose a **template** (e.g., FAQ bot) or start from **scratch**
- Give your bot a **name** and description
- Click **Create**

---

### 3. Design Your Chatbot
- Use the **Flow Editor** to add questions and answers  
- Add **cards**, **actions**, or connect it to **knowledge bases**
- Test your bot in the **emulator**

> 🎯 Tip: You can even train your bot using documents, FAQs, or website URLs

---

### 4. Publish the Bot
- Click on **Share** in the top-right
- Enable **Public Access**
- Copy the **Embed Script** provided by Botpress

---

### 5. Embed in Your Website

Paste the copied script in your `index.html` file right before the closing `</body>` tag:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>My Botpress Chatbot</title>
</head>
<body>

  <!-- Your website content here -->

  <!-- Botpress Chatbot Script -->
  <script src="https://cdn.botpress.cloud/webchat/v0/inject.js"></script>
  <script>
    window.botpressWebChat.init({
      "composerPlaceholder": "Chat with us!",
      "botId": "your-bot-id-here",
      "hostUrl": "https://cdn.botpress.cloud/webchat/v0",
      "messagingUrl": "https://messaging.botpress.cloud",
      "clientId": "your-client-id-here",
      "botName": "SupportBot",
      "stylesheet": "https://your-custom-style.css", // optional
    });
  </script>

</body>
</html>
