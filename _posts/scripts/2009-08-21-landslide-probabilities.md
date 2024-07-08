---
layout: post
title: "Landslide probabilities"
date: "2009-08-21"
tags: [dataset, script]
published: true
image: false
author: Tom Hengl
---

Short title:  landprob

Inputs: DEM in metric projection, Source Landslide areas, H/L value as stopping parameter.  
Outputs: pq\_limi and all other parameters as described in Gruber et al., 2008 article in the Geomorphometry book.

Purpose and use:

Computes Landslide probabilities --- generate landslide probabilities areas using a DEM according to Gruber et al 2008. 
&r landslide1 <dem> <sourcearea\_dem> {h/l stopping value}

**Programming environment**:  Arc AML  
**Status of work**:  Public Domain  
**Reference**:  [Geomorphometry: Concepts, Software, Applications](https://books.google.com.gi/books?id=u33ArNw4BacC&printsec=frontcover&source=gbs_book_other_versions_r&cad=4#v=onepage&q&f=false)
**Data set name**:  [Baranja hill]({{site.baseurl}}/2020/06/30/baranja-hill)

**_Attachment:_**

[landslide_probabilities.zip]({{site.baseurl}}/uploads/datasets/landslide_probabilities.zip)
