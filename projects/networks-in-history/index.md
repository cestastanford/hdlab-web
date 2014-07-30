---
layout: page
title: "Networks in History"
people-tag: neh
presentation-topic: palladio
id: networks-in-history

---


"Networks in History: Data-driven tools for analyzing relationships across time" was awarded $297,137 in July 2013 by the Office of Digital Humanities within the National Endowment for the Humanities under an [Implementation grant](http://www.neh.gov/divisions/odh/grant-news/announcing-6-digital-humanities-implementation-grant-awards-july-2013) for the design and development of visualization techniques to support humanistic inquiry, based on the prototypes created for the <a href="http://republicofletters.stanford.edu">Mapping the Republic of Letters</a> project.


##Process and Products

Our first 'product' released is also an integral part of the ongoing design and development process: [Palladio](/projects/palladio/). Palladio uses the browser (preferably Chrome or Firefox) to let you upload and explore data locally, on your own machine, without sharing that data with anyone. Palladio is also a visualization system that combines a primary view (for example a map, network graph, or even a simple tabular view) with filters to make it easy to query a data set. We start with the assumption that humanities data is multi-dimensional and often has a temporal component. We also assume that queries are often exploratory and heterogeneous rather than formal and hierarchical. Palladio supports our Open Design process. We found in Mapping the Republic of Letters that the visualizations developed were useful only when grounded in specific research questions. In order to develop visualization techniques that support humanistic inquiry more broadly, we need many scholars with a range of case studies to put it to the test and give us feedback. To accomplish this, we have made Palladio available for public use since the very early stages. The design decisions will be driven by the feedback we have from scholars. All the code written for this project will ultimately be open source for those who want to contribute to the project or set up their own instance, but during the development you can consider it Open Use. We do not want to develop behind closed doors and we are not building a black box. Visualization techniques designed by humanists can best serve humanities research. 

### Palladio
### Networks in History Workshop, May 15-16, 2014
We held a workshop May 15-16, 2014 . [Read Mark's workshop summary](http://hdlab.stanford.edu/lab-notebook/palladio/2014/06/23/workshop-summary/).

##Presentations
{% include presentations.html %}

##Core Participants  
<div id="masonry" class="row">
{% for person in site.data.people %}
 {% if person.group contains 'neh' %}
 <div class="col-md-6">
   <div class="well">
    <div class="col-md-3">
<img src="{{ person.image }}" alt="{{ person.name }}" width="80" class="img-rounded">
    </div>
    <div class="col-md-9">
		<h3><a href="mailto:{{ person.email }}">{{ person.name }}</a>
			<br><small>{% if person.neh_role != null %}{{ person.neh_role }}{% else %}{{ person.role }}{% endif %}</small>
		</h3>
    </div>
   </div>
 </div>
{% endif %}
{% endfor %}
</div>






