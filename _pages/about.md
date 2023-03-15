---
layout: about
title: about
permalink: /
subtitle: UC San Diego, Halıcıoğlu Data Science Institute

profile:
  align: right
  image: walker.jpg
  image_circular: false # crops the image to make it circular
  address: >
    <p>walker</p>

news: false  # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false  # includes social icons at the bottom of the page
---
This is a project repository website for DSC 180 - A08

# Background

Living animals are one of the primary sources of data for the development of artificial neural sys- tems. In general, animals are able to perform all of their behaviors and actions under the guidance of a single neural network and its underlying algorithms. One of the end goals for artificial intelligence systems is to emulate these complex neural networks in a virtual manner, to allow our creations to act in a way that replicates how a real animal would behave and learn. Embodied control in neuro- science holds the potential to deepen our understanding of how the real brain works. If a sufficient model of the brain can be created in conjunction with the behaviors that a biorealistically simulated agent generates, then we can quickly generate new hypotheses about real world mappings between the brain and behavior. To achieve this researchers within this field are working to decode all the parts of animals’ neural networks through inferential and replicatory techniques. One of the leading method to do so is to build models to learn how to behave like a real animal, mainly through deep learning models that emulate imitation learning or reinforcement learning. Prior research within this intersection of neuroscience and machine learning have explored methods to solve tasks given input data from a sensory channel, such as vision or sound. The particular approach taken in “Deep Neuroethology of a Virtual Rodent”, along with this replicatory work, focuses on understanding the underlying mechanisms of “embodied control” (Merel et al., 2019), which is how animals utilize a ”combination of their body, sensory input, and behavior” to accomplish tasks, with a particular focus on motor control. The implications of this study include furthering developments in understanding the underlying mechanisms of animal behavior within the fields of motor neuroscience and artificial intelligence.

# Walker Agent Visualization

## Online Model:

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
      <video width="500" height="375" controls autoplay>
      <source src="assets/videos/online_walker.mp4" type="video/mp4">
      </video>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/online_walker.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    LHS is the walker walking, RHS is the walker's states and rewards
</div>

The online model seems to have more unstableness compared

## Behavioral Cloning (BC) Model

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
      <video width="500" height="375" controls autoplay>
      <source src="assets/videos/BC_walker.mp4" type="video/mp4">
      </video>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/BC_walker.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    LHS is the walker walking, RHS is the walker's states and rewards
</div>

# Side-by-side Comparison

<div class="row justify-content-sm-center">
    <div>
      <video width="800" height="600" controls autoplay>
      <source src="assets/videos/TwoAgents.mp4" type="video/mp4">
      </video>
    </div>
</div>
<div class="caption">
    BC Agents is more robust as the kinematic data contain less noise.
</div>

# TSNE Clustering of Kinematics

<div class="row justify-content-sm-center">
    <div>
      <video width="800" height="600" controls autoplay>
      <source src="assets/videos/tsne_sac_walking_highlights_watershed_show_tracks.mp4" type="video/mp4">
      </video>
    </div>
</div>
<div class="caption">
    The TSNE Cluster is loose, indicating inconsistancy of the kinematics
</div>

<div class="row justify-content-sm-center">
    <div>
      <video width="800" height="600" controls autoplay>
      <source src="assets/videos/tsne_bc_walking_highlights_watershed.mp4" type="video/mp4">
      </video>
    </div>
</div>
<div class="caption">
    The TSNE Cluster is dense, indicating the smoothness of the kinematics
</div>


# CKA Analysis

<img src="https://github.com/scott-yj-yang/DSC180-A08/blob/master/assets/img/cka.png" style="display: block; margin: auto;">

