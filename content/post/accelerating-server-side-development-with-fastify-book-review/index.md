+++
title = 'Accelerating Server-Side Development with Fastify by Manuel Spigolon, Maksim Sinik, and Matteo Colina: A Book Review'
date = 2024-05-08T00:00:00-06:00
draft = false
author = "Jose Ortiz"
tags = [
    "Node.js",
    "Fastify",
    "JavaScript",
    "Intermediate",
    "Books"
]
categories = [
    "Book Reviews",
]
series = [
    "Book Reviews",
]
weight = 0
description = 'A review of the book "Accelerating Server-Side Development with Fastify" by Manuel Spigolon, Maksim Sinik, and Matteo Colina, with an overview of the topics the book covers, what I found interesting and remarkable, and what I believe could be improvements for future editions.'
images = ['./images/title-image.jpg']
+++
![Book Cover](./images/book_cover.jpeg 'Cover image source: Packtpub.com')

## Introduction

Recently, the company I work for decided to standardize the use of [Fastify](https://fastify.dev) as the Back-End Node.JS framework for new services (and to migrate existing ones whenever possible). Having not heard of Fastify before (Up to now I had been mostly working with [Express.JS](https://expressjs.com) and dabbled a bit on [Nest.JS](https://nestjs.com) on some POC projects) I started looking for resources to learn about Fastify: What it is, how it works, and it's development paradigm.

After reading the official [Docs and Guides](https://fastify.dev/docs/latest/) provided by Fastify, I found out through [Matteo Colina's](https://nodeland.dev) newsletter (One of Fastify's creators and developers) that the team released a book, **Accelerating Server-Side Development with Fastify**, expanding upon the documentation with in-depth explanations on how Fastify works and good practices when developing Back-End services, so I decided to buy it and learn further about Fastify.

## But first, What is Fastify? 🤔

[Fastify](https://fastify.dev) is a web framework for Node.JS Back-End development focused on low ovehead and high performance. Some of it's features include it being extensible via [Plugins](https://fastify.dev/ecosystem/), efficient logging via the [Pino](https://getpino.io) logger, [TypeScript](https://www.typescriptlang.org) ready, validation of input and output via JSON Schemas, and being one of the faster (If not the [fastest](https://fastify.dev/benchmarks/), depending on when are you reading this 👀) web frameworks. It started development in 2016, had it's version 1 LTS release in 2018 and as of now is currently in version 4 (with version 5 currently in beta).

## The book's content

The book is structured in three sections:

- Fastify Basics
- Build a Real-World Project
- Advanced Topics

The first section is mostly about how Fastify works, it's encapsulation paradigm, lifecycle hooks, routing, plugins, validation via JSON Schemas, and request and response serialization. By the end, you are familiar with most of the inner workings and design decisions behind the Fastify framework.

The second section is where you apply the knowledge learned on the first part by building a To-Do App from scratch, then adding functionality to it, authentication, tests, deploy it to the cloud for it to be accessible everywhere, and finally configuring logs and monitoring tools to keep an eye on the health of your application via [Prometheus](https://prometheus.io).

The last section focuses on advanced topics, including migrating an application from a monolith to a microservice architecture, performance asessment and improvement by bottlenecks and other performance-reducing problems and bugs using various analysis tools, incorporating a [GraphQL](https://graphql.org) API to your project, and using [TypeScript](https://www.typescriptlang.org) to develop Type-Safe apps.

## The Good :+1:

I really enjoyed and learned plenty from the first section of the book, as it explains in a practical way the decisions that were taken when developing Fastify, some general Back-End development good practices, and how you can follow that mindset when building your application to achieve greater performance, easier scalability, and make refactoring down the line more enjoyable as the needs of your application change. As someone that thrives when understanding the way things work internally and the reasoning behind design choices when developing software, I reached the end of the first part better prepared and with a greater understanding of what I could achieve with Fastify. Applying the previous knowledge on a real life project helped to further cement the concepts, and introduced me to tools I hadn’t heard of that are quite useful (And also open source!) like [Prometheus](https://prometheus.io) and [Grafana](https://grafana.com/) for monitoring software. The ‘Performance Assessment and Improvement’ chapter was probably one of my favorites, as it includes a framework to follow to enhance and test your application periodically, together with excellent tools that help you gather data and make an informed decision (That are also open source, BTW 🙌) like [OpenTelemetry](https://opentelemetry.io/), [Zipkin](https://zipkin.io), [AutoCannon](https://github.com/mcollina/autocannon), and [Clinic](https://clinicjs.org/).

## What could be better 🧐

As I believe is normal with first editions, there were a number of typos throughout the book (Good thing they are open to feedback and have a dedicated site to submit them). Also, for better or worse, software evolves constantly, and some of the code examples in the book have since changed or were deprecated on newer versions of Fastify. Fortunately, there’s an up to date [GitHub repository](https://github.com/PacktPublishing/Accelerating-Server-Side-Development-with-Fastify) that is constantly being updated to fix typos, bugs, and outdated dependencies, so I would recommend when in doubt or if a certain piece of code from the book doesn’t quite work (specially if you are working side by side implementing everything instead of just browsing the book) to cross check with the official repository and see if there’s a fix already (Happened to me and in the end it helped).
On a different topic, I consider the last section, ‘Advanced topics’ could be enhanced on a later version. They don’t build on top of the project we did on part 2. Instead, they are different smaller projects. To include these functionalities on the project of part 2 would make the book, in my opinion, an even greater guide.

## Conclusion 🥁

If you are a Back-End developer with previous experience with other frameworks looking to enhance your skills or your app’s performance with Fastify, or even have a little experience with Fastify, this book is a great read, that will give you the tools to become a better Back-End developer, and learn how to make great Fastify apps. Because of the nature of the book, complete beginners or Back-End developers with little experience may face some frustration when trying to follow the book and understand the topics it touches.

Congratulations to [Manuel Spigolon](https://github.com/Eomm), [Maksim Sinik](https://maksim.dev), and [Matteo Collina](https://nodeland.dev) for writing a great book, hoping you can continue to improve it if and when you release a 2nd edition 🎉.

-- Jose

*Accelerating Server-Side Development with Fastify is available on [Amazon](https://www.amazon.com/Accelerating-Server-Side-Development-Fastify-comprehensive/dp/1800563582/ref=tmm_pap_swatch_0?link_from_packtlink=yes), [Packt](https://www.packtpub.com/product/accelerating-server-side-development-with-fastify/9781800563582), and [O'Reilly](https://www.oreilly.com/library/view/accelerating-server-side-development/9781800563582/?_gl=1*1bexho7*_ga*MTIyOTM1MjU1MS4xNzE1NDg1MjI2*_ga_092EL089CH*MTcxNTQ4NTIyNi4xLjAuMTcxNTQ4NTIyOC41OC4wLjA.) (Via their learning platform).*

## Further Reading/Watching

- [The Fastify Framework](https://fastify.dev)
- ['Take your http server to ludicrous speed' talk by Matteo Collina (Video)](https://www.youtube.com/watch?v=5z46jJZNe8k)