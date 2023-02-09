# API-ChatGPT-Java

[![LinkedIn Badge](https://img.shields.io/badge/LinkedIn-Profile-informational?style=flat&logo=linkedin&logoColor=white&color=0D76A8)](http://www.linkedin.com/in/paulabadt)
![GitHub contributors](https://img.shields.io/github/contributors/Paulabad-BigData/API-ChatGPT-Java)
![GitHub follow](https://img.shields.io/github/followers/Paulabad-BigData?style=social)
![GitHub stars](https://img.shields.io/github/stars/Paulabad-BigData/API-ChatGPT-Java?style=social)
![GitHub forks](https://img.shields.io/github/forks/Paulabad-BigData/API-ChatGPT-Java?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/Paulabad-BigData/API-ChatGPT-Java?style=social)

## How to get it running

- Clone this GIT project.
- Make sure it is a Maven project and Maven is executed to load dependencies.
- Create an Account at https://openai.com & log in
- Create API key at https://beta.openai.com/account/api-keys
- Store the key in application.properties file in cloned project.
- Start it as Spring Boot application.
- For chatting with ChatGPT: http://localhost:8080/
- For drawing images with DALL-E: http://localhost:8080/image

## Setup proxy

If you need a proxy to communicate with Internet (ChatGPT API is in Internet), adapt ChatGptController.java like this:

- Replace: private HttpClient client = HttpClient.newHttpClient();
- with: private HttpClient client = HttpClient.newBuilder().proxy(ProxySelector.of(InetSocketAddress.createUnresolved("proxy.host.com", 8080))).build();

## More information

OpenAI API documentation: https://beta.openai.com/docs/api-reference/completions/create
