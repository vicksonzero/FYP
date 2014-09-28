## Background

It is common for graphics designers to design website mock-ups in graphics software before actually coding them. This saves them time drilling into front-end coding and they can focus on the visual design rather than the underlying code. However, designers nowadays often need to produce designs not only for desktop and smartphones, but for all sorts of device sizes. In other words, they have to produce multiple drawings for a responsive website.

Usually, the drawings should have already sufficient information about the outcome of the website. It is redundant to repeat the building of the website in HTML, given that all graphic components are already present. 

If there exists a tool that transforms a website drawing into a basic responsive website, it will save the designer plenty time revisiting the draft drawings for the metrics, colors and details. 

## Project Scope

In this scenario, the most challenging part is for the tool to recognize the different layout given arbitrary transformations, additions, and/or omissions. If the tool can correctly recognize the features from each designs, the rest are simple calculations and html/css implementations.

Therefore, this project will only try to correctly identify similarities between different versions of the same website, given that they have similar contents.

This project will also limit to a single-page website. There will be no restrictions in the number of sections in it.

Since vector graphics are more readily editable, we will just focus in website drawings in svg, an XML format for describing vector graphics.

## Problem Statement

Given 2 scalable vector graphic (svg) files, list and track their similarities and differences, so that the other file will change accordingly when one of them changes.

## Project Objectives

1. To recognize symbol groupings within a drawing and to track the change of groupings

2. To tell if the same symbol appears in other drawings or not.

3. To actively edit other drawings if a change is made to only one of the drawings.


## Major technical components

1. To recognize meaningful graphic components from unorganized vector graphic hierarchies.

2. To recognize similarities between symbols involving transformations, addition or omission.

## Expected results & deliverable

A Side-by-side vector graphic editor that has two windows next to each other. When the user commits the changes in one side, the other side will have similar changes applied, selectively, according to whether the feature appears on it.


## Project schedule

1. [Obj-1] Simplify an svg file to a tree of symbols, By mid November
1. [Obj-2] Identify similarities in a well-formed svg file, By the end of January
1. [Obj-2] Identify similarities in the tree of symbols, By the end of February
1. [Obj-3] Utilize similarity data to edit respective places in the other file, By mid May
1. [Obj-3] Write up a demonstrational svg editor, By the end of May
1. [Other] Bug fix, Before June


##Background reading

Kim, B. & Yoon, J. P. (2005). Similarity measurement for aggregation of spatial objects.. In H. Haddad, L. M. Liebrock, A. Omicini & R. L. Wainwright (eds.), SAC (p./pp. 1213-1217), : ACM. ISBN: 1-58113-964-0

Sciascio, E. D., Donini, F. M. & Mongiello, M. (2004). A Logic for SVG Documents Query and Retrieval..Multimedia Tools Appl., 24, 125-153. 
