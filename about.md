---
layout: default
title: About Me
---

<div class="post">
	<h1 class="pageTitle">About Me</h1>

	<p class="intro">I am a senior scientist leading in the SciML team based at Rutherford Appleton Laboratory. SciML is a team in the Scientific Computing Division and we work with the large STFC facilities (Diamond, ISIS Neutron and Muon Source and Central Laser Facility for example) to use machine learning to push the boundaries of fundamental science.</p>
	
	<p class="intro">My interests lie in developing machine learning approaches for materials science. I have experience leading projects to apply deep neural networks as well as classical machine learning (eg support vector machines) as well as atomistic simulation (eg DFT) to projects in materials characterisation and design. I have more than 10 years experience collaborating with experimental researchers to use computational tools for accelerated and advanced analysis of results.
	</p>
	
<figure>
	<img src="{{ '/assets/images/photoferroics-small.png' | prepend: site.baseurl }}" alt="" width="700" > 
	<figcaption>Fig1. Mechanisms for the ferroelectric photovoltaic effect, taken from the article "Ferroelectric materials for solar energy conversion: photoferroics revisited".</figcaption>
</figure>
	
  <h2>Projects</h2>
  
<h3>Machine Learning for Inelastic Neutron Scattering</h3>

We are developing interpretable, calibrated machine learning techniques for the analysis of inelastic neutron scattering data. This work is in collaboration with ISIS neutron and muon source. This work was recently highlighted by the British Computing Society [here](https://www.bcs.org/content-hub/ai-the-next-big-thing-for-accelerating-materials-science-experiments/?utm_campaign=BCS%20Articles&utm_content=153369529&utm_medium=social&utm_source=linkedin&hss_channel=lcp-25323)

Also see my AI3SD webinar presentation
<a href="https://www.ai3sd.org/2020/12/16/16-12-2020-ai3sd-winter-seminar-series-enhancing-experiments-through-machine-learning/">here </a>


<h3>Machine Learning for X-ray Tomogrpahy</h3>

This is work funded by Innovate UK, in association with Finden Ltd. We have been developing deep learning methods to reconstruct 3D maps of XRD patterns, allowing analysis of complex materials structures over unprecedented length scales and with unprecedented time resolution - opening up the potential for in situ observation of complex chemical phenomena in 3D.

Collaborator Prof. Andy Beale presents the power of XRDCT <a href="https://ukcatalysishub.co.uk/webinar-prof-andrew-beale-professor-of-inorganic-chemistry-dept-of-chemistry-ucl-finden-ltd/">here </a> 

<h3>Machine Learning for X-ray Electron Microscopy</h3>

Working on projects with <a href="https://www.diamond.ac.uk/Instruments/Imaging-and-Microscopy/ePSIC.html">ePSIC </a> and also <a href="https://matthey.com/en">Johnson Matthey </a> we are building machine learning tools to enhance, accelerate and automate the operation of some of the world's most powerful electron microscopes.

<h3>Machine Learning for Accelerated Materials Design</h3>

In collaboration with Aron Walsh at Imperial College London and Ricardo Crespo at the University of Reading we are developing descriptors, and tools for machine learning the properties of materials, from crystal structure prediction to property estimation. 
<a href="https://github.com/a-ws-m/unlockGNN">Unlock GNN</a> allows use of modern graph neural networks to make use of knowledge about structure in the estimation of materials properties. When applied with 
<a href="hhttp://smact.readthedocs.io/en/latest/introduction.html">SMACT</a> this allows the construction of high-throughput design workflows for functional materials discovery.

  <h2>Software</h2>
  
 During the past few years I have been leading development of and applying tools for materials science. These tools are available under open source licenses on <a href='https://github.com/keeeto/'>my GitHub page.</a>

	
	<h3>SMACT</h3>
	
	<img align="left" hspace="20" src="{{ '/assets/images/smact-toc.jpeg' | prepend: site.baseurl }}" alt="" width="200"> 
	
<a href="http://smact.readthedocs.io/en/latest/introduction.html"> SMACT </a>stands for Semiconducting Materials from Analogy and Chemical Theory. It is a set of tools to use simple chemical descriptors, statistical models and high-throughput workflows to discover new materials. SMACT is written in simple modular Python and allows users to develop their own models and workflows using the basic machinery provided. In recent years we have had our first publications exploring the vast hyperspace of hitherto un-reported materials. I wrote a bit more about these in another post.

   <h3>Superres-tomo </h3>
   
   	<img align="right" hspace="20" src="{{ 'https://superres-tomo.readthedocs.io/en/latest/_images/cnn-reconstruct.png' | prepend: site.baseurl }}" alt="" width="200"> 
   	
   	<a href="https://superres-tomo.readthedocs.io/en/latest/about.html">superres-tomo</a> is a package of useful scripts and models for applying neural networks for tomographic reconstruction of X-ray images. The package also includes models and scripts useful for the analysis of the images generated, allowing tasks such as semantic segmentation of very large images and removing noise from low dose images.
   
	
	<h3>Macrodensity</h3>
	
	
	<img align="right" hspace="20" src="{{ 'https://github.com/keeeto/BandAlignmentBootcamp/raw/master/hybrid_bands.jpeg' | prepend: site.baseurl }}" alt="" width="200"> 
	
	<a href="https://github.com/WMD-group/MacroDensity">MacroDensity</a> s a set of tools for analysing and manipulating electron densities obtained from quantum mechanical calculations of materials. This is useful for finding electron binding energies, aligning bands, calculating defect levels and many other properties. I explain how to use MacroDensity in a <a href="https://github.com/WMD-group/MacroDensity/tree/master/tutorials"> series of tutorials</a>, available as iPython notebooks. 
	</div>
	
<h2>Food</h2>
<img align="right" hspace="20" src="{{ 'http://fodblog.github.io/assets/pictures/caprese_omlette.jpg' | prepend: site.baseurl }}" alt="" width="300">

In my spare time I do a lot of exploring food, eating and making. For several years before my science jobs I worked in kitchens, ranging from stacking the back of hot food <a href="https://en.wikipedia.org/wiki/FEBO">"Febo" style</a> vending machines, to the five star <a href="http://cafeamericain.nl/">Hotel Americain</a>. 

<img align="left" hspace="20" src="{{ 'http://fodblog.github.io/assets/pictures/baked-egg-kale.jpg' | prepend: site.baseurl }}" alt="" width="300">

I'm currently pretty obsessed with pickling and fermenting. I am working on my pickled eggs and kimchi. I write a regular food blog, which is also focussed on Fodmap-frinedly recipes. Fodmap means that the recipes are suitable for people with IBS, you can find more <a href="https://fodblog.github.io/">on the FodBlog</a>. 
