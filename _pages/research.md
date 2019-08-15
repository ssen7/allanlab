---
title: "AI in Gastroenterology Group - Research"
layout: research
excerpt: "AI in Gastroenterology Group -- Research"
sitemap: false
permalink: /research/
---

### Visual recognition and understanding of Gastrointestinal diseases

Deep learning methods for medical diagnostic imaging can reduce delays in diagnosis and give improved accuracy rates over other analysis techniques. We focuse on methods with applicability to automated diagnosis of images obtained from gastrointestinal biopsies. These deep learning techniques for biopsy images may help detect distinguishing features in tissues affected by enteropathies. Learning from different areas of an image, or looking for similar patterns in new images, allow for the development of potential classification or clustering models Techniques like these provide a cutting-edge solution to detecting anomalies. In this paper we explore state of the art deep learning architectures used for the visual recognition of natural images and assess their applicability in medical image analysis of digitized human gastrointestinal biopsy slides. Pathology has played an essential role in diagnosing gastrointestinal disorders. However, errors can occur due to complex systems, time constraints and variable inputs. This can be further complicated when the biopsy images share histological features. Computational methods have the potential to address these challenges. In light of this, developing assistive computational methods can help mitigate said errors. The goal of applying computational methods in identifying diseases is for developing fast, reproducible and reasonably accurate methods that can be easily standardized.

### Computational image analysis to address staining color bias in duodenal biopsies
Hematoxylin and Eosin(H&E) stains are the most widely used stains in medical diagnosis. Digital images used in computational pathology may contain significant variations in H\&E staining due to a number of factors. These factors include differences in tissue preparation, raw materials, manufacturing protocol, and digital scanners. The variations of stain color in groups of images can create a bias in deep learning models such as Convolutional Neural Networks. Color correction techniques are applied to H\&E stained images to attempt to remove the potential biases from staining variations. In this paper, we compare the performance of three different color normalization techniques when applied to a deep learning classification model. The techniques tested are structure-preserving color normalization, a non-linear mapping approach to stain normalization, and color balancing. The classification dataset consists of duodenal biopsy images originating from three different sources and contains Celiac Disease, Environmental Enteropathy, and Normal classes. After pre-processing images with each color correction technique, the images are classified using an equivalent training set and deep learning architecture.

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}

<div id="comparison">
  <figure>
    <div id="divisor">
    </div>
  </figure>
  <input type="range" min="0" max="100" value="50" id="slider" oninput="moveDivisor()">
</div>

<script>
  var divisor = document.getElementById("divisor"),
    slider = document.getElementById("slider");
  function moveDivisor() {
    divisor.style.width = slider.value + "%";
  }
</script>