---
title: 'Layered DAG drawing - list of useful reading'
date: 2019-01-18
permalink: /posts/2019/01/DAG-drawing/
tags:
  - Graph drawing
  - Mapper
  - visualization
  - WIP
---
I decided to add a layered graph drawing algorithm to my Mapper code [citation missing]
So i have been looking for descriptions of the Sugiyama Method online, here are the best i found:  
  <https://github.com/erikbrinkman/d3-dag>  
  <https://www.csd.uoc.gr/~hy583/papers/ch10.pdf>  
  <http://www.it.usyd.edu.au/~shhong/fab.pdf>  
  <http://publications.lib.chalmers.se/records/fulltext/161388.pdf>  
  <http://www.graphviz.org/Documentation/TSE93.pdf>  
  <https://blog.disy.net/sugiyama-method/>  
  <https://pdfs.semanticscholar.org/9d5e/62920365f339e9121e6e62f4cdc7a10ed058.pdf>  

The Sugiyama Method consists of 4 Steps:
1. Cycle Removal
2. Layer Assignment
3. Vertex ordering
4. Coordinate Assignment

The first issue with applying a DAG based method to a Mapper built graph is that mapper graphs are not directed. What we can do is consider the direction to be induced by the monotonic variation in the filter chosen for the construction of the graph. The directed graph constructed this way is going to be acyclic by construction of the mapper algorithm. Therefore, Step 1. is now superfluous.   
The filter information of the Mapper does not only come handy for assigning direction to the undirected edges in the graph, but also with completing Step 2. of the Sugiyama method: Layer Assignment. In our visualization of the Mapper we want to highlight the levels of construction of the graph. Hence, we can assign a layer to each bin. This is rather useful since, by construction, the nodes in each bin are not connected with each other.  

The Sugiyama Method for Mapper consists of 2 Steps:
1. Vertex ordering
2. Coordinate Assignment

More updates as I learn more and fully develop the algorithm ... 
