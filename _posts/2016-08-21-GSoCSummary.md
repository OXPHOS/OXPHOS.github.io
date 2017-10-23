---
layout: post
title:  "GSoC'16 Summary"
date:   2016-08-21 13:29:31 -0400
---

I worked with [Shogun Machine Learning Toolbox](https://github.com/shogun-toolbox/shogun) as a part of the [Google Summer of Code Program](https://developers.google.com/open-source/gsoc/) during the past summer. Shogun is an open source software written mostly in C++, and supports machine learning algorithms via interfaces to many languages, including Python, R and Java. It has been developed for ten years and tens of contributors should be credited for the constant improvement of the package. It is a great honor that I can also be part of it and contribute to the project.


My work during the summer mainly composed of three parts. First, I helped with the new linear algebra library in Shogun. Linear algebra computation provides backend supports for machine learning. Thus, an efficient and convenient internal linear algebra library benefits a lot. With the discussion and guidance from [Heiko](https://github.com/karlnapf), [Rahul](https://github.com/lambday) and [Viktor](https://github.com/vigsterkr), we successfully set up the new header-only, plug-in based linear algebra library, which enables both CPU and GPU linear algebra operations.


Second, I refactored the serialization framework in Shogun with `Cereal` library, mentored by Heiko and Viktor. `Cereal` library is a header-only C++11 serialization library that is fast, light-weight, and easy to extend. We coded the interface that enables serialization of the new tag parameter framework in Shogun with `Cereal`, which allows easy and readable archive of Shogun data.


And last, I wrote 13 cookbook pages with API examples of different machine learning algorithms. The cookbook project aims to illustrate the algorithms used in Shogun in all target languages and provide easy-to-read instructions for new users to Shogun. While coding up the examples, I learned several machine learning algorithms I was not familiar with before. 


I have accomplished a more technique-based [summary](https://github.com/OXPHOS/shogun/wiki/GSoC-2016-Final-Report-:-The-Shogun-Detox) on Github with the links to the work I have been doing. Also, the detailed introduction about the [linear algebra library](https://github.com/OXPHOS/shogun/wiki/README_linalg_refactor) and [serialization framework](https://github.com/OXPHOS/shogun/wiki/README_cereal) can be found on wiki. 


Apart from machine learning theories, I gained a lot experience with coding techniques and philosophy.  As a student who does not major in computer science, I had no experience with the huge projects like Shogun. I spent time reading the codes and trying to understand the structure of Shogun as my first step. Thanks to the neat organization of Shogun scripts and the patience from Shogun members, I started to appreciate the principles for framework design. I also touched on GPU calculation and serialization, which are basic but important functions for a real world project. I was able to put the concepts I read in the textbooks into practice, such as smart pointers and opaque pointers, as well. 


There was moment when I was frustrated by the knowledge I knew nothing about or the problems I failed so many times to solve, but I am glad I didn’t give up and finally made things through. I could not finish the work without my mentors, Heiko, Rahul and Viktor. They are always patient with my various sorts of questions. I am also grateful to have [Sergey](https://github.com/lisitsyn) and Lea on the team, who are always ready to help. [Saurabh](https://github.com/Saurabh7) and [Sanuj](https://github.com/sanuj) are my peers who also joined Shogun via GSoC program. Their enthusiasm motivated me a lot. 


People are making choices and giving up other options all the time, and the past summer was the experience I won’t regret to have. It was intense, but also fruitful and enjoyable. For the students who want to join and get the most out of the summer program, I just have one tip to share, and for myself to remember: be inspired and devoted. I promise you will have a summer as wonderful as I did.
