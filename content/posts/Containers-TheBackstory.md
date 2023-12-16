+++
title = 'Containers: The Backstory'
date = 2023-08-30T22:53:30+01:00
description = "About the containers' history"
tags = ["containers", "docker", "kubernetes"]
type = 'post'
+++

Back in my student days, I first bumped into Docker. It was all the rage then, and honestly, it blew my mind. The idea that you could take a piece of code, make it work anywhere in its own little space, separate from the computer's main system – that was pretty cool. Later on, I found out Docker wasn't the first to come up with this container and isolation stuff. In this blog post, I want to take you on a little trip back in time to check out who started it all. Let's explore the early days of container technology together!


## The Foundations: Chroot

All started in 1979, with the chroot command in Unix V7. What's chroot, you ask? It's a neat little trick that lets processes switch up their root directory, making a kind of separate area for them to run in. Sure, chroot wasn't exactly a container solution like we think of now, but it was a huge leap towards keeping processes isolated. Think of it as the first building block in the world of container technology!

## Solaris Zones and Jails

Zooming ahead to the early 2000s, the scene starts to get even more interesting. Enter FreeBSD Jails – this was like an upgrade to the old chroot idea. Jails took things up a notch by offering a fancier setup for keeping processes in their own spaces. Meanwhile, over at Sun Microsystems, they were cooking up something called Solaris Zones. This was pretty cool stuff; it let different OS instances coexist on the same physical host, all under one roof!


## Linux Containers

In 2008 LXC (Linux Containers) entered the scene. LXC was a big deal because it brought together cgroups (control groups) and namespaces – two handy features from the Linux kernel. Which created a lighter, more efficient way to do virtualization. Basically, LXC made it possible to run processes in their own isolated spaces, and that's a big step toward the container technology we use today. And guess what? In future blog posts, we're going to dive deep into cgroups and namespaces, so stay tuned for that!

## Docker Era

While LXC was innovative, it wasn't until Docker's launch in 2013 that containers became mainstream. Docker offered a high-level tool with an easy-to-use interface, enabling developers to package, distribute, and manage applications within containers efficiently. The introduction of Docker Hub, a cloud-based registry service, further fueled the adoption of container technology.

## The Rise of Orchestration with Kubernetes

As more and more apps started using containers, there was a huge need for something to keep all these containers in check. That's where Kubernetes comes into the picture in 2014. Driven by Google and then passed to the Cloud Native Computing Foundation (CNCF), Kubernetes turned into the backbone of container orchestration. What's so great about it? It makes deploying, scaling, and managing containerized apps efficiently. Basically, Kubernetes is like the maestro, making sure every container is playing its part perfectly in the grand orchestra of applications.

## Beyond Docker: Container Runtimes

Docker's success sparked the birth of container runtimes like `containerd` and `cri-o`. Each of these tools offered varied functionalities, and they played a big part in shaping the Open Container Initiative (OCI). What's OCI all about? It's focused on setting up standard rules for how container formats and runtimes should work. Think of it like a bunch of tech folks agreeing on how to make containers play nice together, no matter who builds them.

## Conclusion

Starting from simple beginnings with `chroot` to a whole evolving ecosystem built around Docker and Kubernetes, it's incredible how far containers have come. Looking ahead, it's clear that containers, with all their perks like portability, efficiency, scalability, are going to stay right at the heart of tech growth and the way we roll out software. It's an exciting journey, and who knows what cool stuff we'll see next!