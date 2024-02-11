# Spring AI


* [Spring AI Docs](https://docs.spring.io/spring-ai/reference/)

* [Spring AI Project](https://github.com/spring-projects/spring-ai)



The Spring AI library is a set of APIs and components that allow Java developers to integrate artificial intelligence (AI) into their Spring Boot applications. The library is based on the Spring Framework and provides a unified API to access a variety of AI technologies, including machine learning, deep learning, natural language processing, and computer vision.

Spring AI provides a number of features to make it easy to integrate AI into Spring Boot applications. These features include:

Support for a variety of AI technologies: Spring AI supports a variety of AI technologies, including machine learning, deep learning, natural language processing, and computer vision. This allows developers to choose the AI technology that best meets their needs.
Unified API: Spring AI provides a unified API to access all AI technologies. This simplifies the development of Spring Boot applications that integrate AI.
Ease of use: Spring AI is designed to be easy to use. Developers can start using the library quickly, without the need to learn a new API.
Spring AI can be used for a variety of purposes, including:

Recommendations: Spring AI can be used to generate personalized recommendations for users, based on their historical data.
Data analysis: Spring AI can be used to analyze data and identify patterns and trends.
Anomaly detection: Spring AI can be used to detect anomalies in data, such as fraud or cyber attacks.
Natural language processing: Spring AI can be used to process natural language, such as translation, summarization, and text generation.
Computer vision: Spring AI can be used to process images and videos, such as object identification, image classification, and facial recognition.
Spring AI is a powerful tool that can help developers integrate AI into their Spring Boot applications. The library is easy to use and provides support for a variety of AI technologies.

Here are some additional details about the Spring AI library:

* The library is still under development, but it has already been used in a variety of production applications.
* The library is open source and available on GitHub.
* The library documentation is available on the Spring website.

# Project Setup

When configuring your Maven pom.xml for the Spring AI project, add the specified repository to access its dependencies. As Spring AI is currently in the experimental phase, only snapshot versions are available. Here is how you should include this in your pom.xml:

```
<repositories>
        <repository>
            <id>spring-snapshots</id>
            <name>Spring Snapshots</name>
            <url>https://repo.spring.io/snapshot</url>
            <releases>
                <enabled>false</enabled>
            </releases>
        </repository>
    </repositories>
```

In this project, I have selected OpenAI as the primary interface. However, it's important to note that Spring AI offers a variety of different ChatClient interfaces.

* OpenAI
* Azure OpenAI
* Hugging Face
* Ollama

OpenAI Library
```
<dependency>
  <groupId>org.springframework.ai</groupId>
  <artifactId>spring-ai-openai-spring-boot-starter</artifactId>
  <version>${spring-ai.version}</version>
</dependency>
```
PDF Document Reader (ETL)
```
<dependency>
  <groupId>org.springframework.ai</groupId>
  <artifactId>spring-ai-pdf-document-reader</artifactId>
  <version>${spring-ai.version}</version>
</dependency>
```
Vector Database(PGvector) 
```
<dependency>
  <groupId>org.springframework.ai</groupId>
  <artifactId>spring-ai-pgvector-store</artifactId>
  <version>${spring-ai.version}</version>
</dependency>
```

The most recent version of this library is 0.8.0-SNAPSHOT.

After all setup, you need to create your account and API key in one of the chosen clients. In my case [OpenAI Platform](https://platform.openai.com/docs/overview)

This was just the first study with Generative AI and the Spring AI library. We will develop some other features using the library, and I hope you follow my journey with Spring and AI.

Part of this doc was generated with SpringAI and Model ChatGPT 3.5.

![Spring IA API response](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/yi9dfqbsz24sihqlc00d.png)
