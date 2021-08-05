---
title: Dockerize me up!
date: "2021-08-01T22:40:32.169Z"
description: We need Docker fist of all. Make sure you have it installed before proceeding
---

Docker is a container platform that enables companies to build, share and run any application, from almost any location possible. Almost every company is packaging their applications for faster production workloads, so they can deploy at any time with no extra costs. There are many ways we can build a React application, One way is to dockerise the React application with the **nodeJs** backend and create a docker image so that we can deploy that image.

### Technologies Used in this post:

- **React**: It is a JavaScript library created by Facebook to build User Interfaces. You can find more information at [reactjs.org](https://https://reactjs.org/).

- **Docker**: It is a tool designe4d to facilitate the creation, implementation and execution of apps through the use of containers. In this case it will allow us to package a React application with all its libraries and dependencies and send it as a package. This will ensure that it will work on any machine that has docker installed. You can read more about it [clicking here](https://www.docs.docker.com).

- **Nginx**: It is an open source software for web serving, reverse proxy, caching and/or load balancing. It started as a web server deswigned for maximum performance and stability. In addition to its **HTTP** server capabilities, NGINX can also function as a proxy server for email (such as IMAP, POP3 and SMTP) and reverse proxy/ load balancer for HTTP, TCP and UDP servers. Learn more by [clicking here](https://nginx.org/en/docs)

## Installing Docker

Installing Docker Descktop on a Mac is pretty straight forward. We need to go to [this link](docs.docker.com/docker-for-mac/install/) and download the image for our machine.

In order to check if the installation has been successfull we can run the next commands in the terminal:

```
docker info
docker --version
```

## Creating a web app by using React

1. Our first step is to install by using yarn, our package `create-react-app`

```
yarn add create-react-app
```

2. Next thing we need to do is by using the command `create-react-app`, we can create our React app. We call this app 'test-docker'

```
npx create-react-app test-docker
```

3. And cd into our directory so that we can execute our app

```
cd test-docker && yarn start
```

## Steps to follow

As we have seen above, Docker makes it easy for developers to package, ship and run any application as a self-contained, portable, lightweight container that can run virtually any application.Docker containers are also easy to deploy in the cloud. We are going to create

<!-- https://www.ionos.es/digitalguide/servidores/configuracion/tutorial-docker-instalacion-y-primeros-pasos/ -->

<!--
The Big Oxmox advised her not to do so, because there were thousands of bad
Commas, wild Question Marks and devious Semikoli, but the Little Blind Text
didn’t listen. She packed her seven versalia, put her initial into the belt and
made herself on the way.

- This however showed weasel
- Well uncritical so misled
  - this is very interesting
- Goodness much until that fluid owl

When she reached the first hills of the **Italic Mountains**, she had a last
view back on the skyline of her hometown _Bookmarksgrove_, the headline of
[Alphabet Village](http://google.com) and the subline of her own road, the Line
Lane. Pityful a rhetoric question ran over her cheek, then she continued her
way. On her way she met a copy.

### Overlaid the jeepers uselessly much excluding

But nothing the copy said could convince her and so it didn’t take long until a
few insidious Copy Writers ambushed her, made her drunk with
[Longe and Parole](http://google.com) and dragged her into their agency, where
they abused her for their projects again and again. And if she hasn’t been
rewritten, then they are still using her.

> Far far away, behind the word mountains, far from the countries Vokalia and
> Consonantia, there live the blind texts. Separated they live in Bookmarksgrove
> right at the coast of the Semantics, a large language ocean.

It is a paradisematic country, in which roasted parts of sentences fly into your
mouth. Even the all-powerful Pointing has no control about the blind texts it is
an almost unorthographic life One day however a small line of blind text by the
name of Lorem Ipsum decided to leave for the far World of Grammar.

### According a funnily until pre-set or arrogant well cheerful

The Big Oxmox advised her not to do so, because there were thousands of bad
Commas, wild Question Marks and devious Semikoli, but the Little Blind Text
didn’t listen. She packed her seven versalia, put her initial into the belt and
made herself on the way.

1.  So baboon this
2.  Mounted militant weasel gregariously admonishingly straightly hey
3.  Dear foresaw hungry and much some overhung
4.  Rash opossum less because less some amid besides yikes jeepers frenetic
    impassive fruitlessly shut

When she reached the first hills of the Italic Mountains, she had a last view
back on the skyline of her hometown Bookmarksgrove, the headline of Alphabet
Village and the subline of her own road, the Line Lane. Pityful a rhetoric
question ran over her cheek, then she continued her way. On her way she met a
copy.

> The copy warned the Little Blind Text, that where it came from it would have
> been rewritten a thousand times and everything that was left from its origin
> would be the word "and" and the Little Blind Text should turn around and
> return to its own, safe country.

But nothing the copy said could convince her and so it didn’t take long until a
few insidious Copy Writers ambushed her, made her drunk with Longe and Parole
and dragged her into their agency, where they abused her for their projects
again and again. And if she hasn’t been rewritten, then they are still using
her. Far far away, behind the word mountains, far from the countries Vokalia and
Consonantia, there live the blind texts.

#### Silent delightfully including because before one up barring chameleon

Separated they live in Bookmarksgrove right at the coast of the Semantics, a
large language ocean. A small river named Duden flows by their place and
supplies it with the necessary regelialia. It is a paradisematic country, in
which roasted parts of sentences fly into your mouth.

Even the all-powerful Pointing has no control about the blind texts it is an
almost unorthographic life One day however a small line of blind text by the
name of Lorem Ipsum decided to leave for the far World of Grammar. The Big Oxmox
advised her not to do so, because there were thousands of bad Commas, wild
Question Marks and devious Semikoli, but the Little Blind Text didn’t listen.

##### Wherever far wow thus a squirrel raccoon jeez jaguar this from along

She packed her seven versalia, put her initial into the belt and made herself on
the way. When she reached the first hills of the Italic Mountains, she had a
last view back on the skyline of her hometown Bookmarksgrove, the headline of
Alphabet Village and the subline of her own road, the Line Lane. Pityful a
rhetoric question ran over her cheek, then she continued her way. On her way she
met a copy.

###### Slapped cozy a that lightheartedly and far

The copy warned the Little Blind Text, that where it came from it would have
been rewritten a thousand times and everything that was left from its origin
would be the word "and" and the Little Blind Text should turn around and return
to its own, safe country. But nothing the copy said could convince her and so it
didn’t take long until a few insidious Copy Writers ambushed her, made her drunk
with Longe and Parole and dragged her into their agency, where they abused her
for their projects again and again. -->
