---
layout: post
title: Computer Vision and Lake Malawi Cichlids
header-img: "img/Cichlid-Peacock-OB.jpg"
---

As someone who is both interested in computer vision, but also has had cichlids in their aquarium before, I thought [this article](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0077686) was pretty cool.

Basically, it appears that they can classify a particular species both by its particular morphology and color. The interesting tid bit is that they found that you could identify, at least reasonably well (67% success with RGB+HSV extraction method), a particular species based on the three primary color groups in the sample. Using the Python OpenCV library they were also able to classify features of their coloration; i.e. stripes.

In the end they found, "that the average success rate of accurate
classification by naked human eye was 41.6%." Considering the success of this, I wonder if this technique could be applied to any other species. Perhaps finches?
