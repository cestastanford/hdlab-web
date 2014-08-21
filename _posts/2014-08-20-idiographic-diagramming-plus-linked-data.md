---
layout: post
title:  "Idiographic Diagramming Tool for Linked Data Exploration, Editing and Creation"
author: Nicole Coleman
date:   2014-08-20 16:00
category: piranesi
published: true
tags: 
excerpt: "These are preliminary ideas about interface elements and interaction based on use cases for the Humanities+Design/Grand Tour course. This is our test case for applying the idiographic diagramming tool to linked data exploration and creation. The process also involves creating scholarly schema through the research process as a research outcome."

---


An idiographic approach to data visualization and the construction of diagrams to support the research process. Navigation of three-dimensional data model by exploring one entity type at a time. 

##Three Primary Views

###1. Graph
**Spatially orient entities for "thinking through data."**  
The graph view is better described as a workspace. The graphic elements are nodes and lines that act as links between the nodes. The purpose of the graph workspace is to allow researchers to explore, edit and create entities and attributes in the form of groupings, connections, and tags. Nodes can also be merged. Attributes can be added to links.  

A number of pre-defined layouts can be applied to the nodes in the Graph View, but the assumption is that researchers will use the space to spatially orient the nodes themselves. 

###2. Data
**A detailed view of each object and its attributes.**  
The data view is an elegant and easily readable representation of the entities and their attributes as objects. The data view is an editing interface that is synchronized with the graph view. Create a new entity in the data view, produces a node in the graph view and in the Palette. 

The data view and the graph view complement each other. One provides feedback on actions taken in the other. Both the Data View and the Graph View 

###3. Palette
**Overview of complete data set as entities, grouped by entity type.**  
The palette gives us the opportunity to see all of the data at one view. Selections can be made from the Palette and dragged into the graph view for editing, organizing, and categorizing. The denity is adjustable to the pixel level for handling very large data sets.

![image](http://drive.google.com/uc?export=view&id=0B1XIzIvpOWe4aTY5Zk9CYmhNZms)

##Interactions between panels
1. Selection
	> Double-click to select in Graph. Entity highlighted in Palette.
2. Merging
	>Merge nodes/entities in Graph. Immediately updated in Data and Palette.
3. Editing
	> Modifying the entity type for one node in Data view or Graph view. Modify Entity type for a number of nodes in Palette. Same for attributes. Example: 
4. Create node
	>Node created in Graph without entity-type specified appears in Palette as gray. It appears in Data in light type as undefined.
5. Shifting entity type view
	> A shift from 'people' to 'places' in the Graph view will, be default, show all of the 'places' entities that are linked to the 'people' entities. While inelegant, this would make it possible to navigate through the different dimensions of the data while keeping some consistency in terms of the selection of data being viewed.

##Use Cases
We decided to narrow the development scope initially to use cases for a course that will be taught this fall (2014) on the Grand Tour. The core text for the course is the _Dictionary of British and Irish Travelers on the Grand Tour in Italy, 1701-1800_. A digitized copy of the text has been carefully chunked by entry (basically one entry for each traveler) and then each entry parsed to extract biographical details, tours in Italy, and cities visited. The Grand Tour Explorer is an online tool for exploring and querying this digitized and parsed text. The students can use the Explorer to select all of the entries that include visits to Genoa, for example, and then export that subset of entries (or the sparQL query) and work with them in another context such as the Idiographic Diagramming Tool or Palladio. 

###1. Curating the Grand Tour Data Set
**Add relationships between existing entities.**
We have parents identified by name for many people, but not matched to existing entities. A search in the Palette for the parent name would reveal the matching entity (or duplicates). Drag to the Graph and make the connection.

**Add new entities.**
Entries in the dictionary are not people. We could generate people entities out of the entries by creating, for example, two people-type entities: Mr. Haversham and Mrs. Haversham linked to the entry-type entity.

###2. Generating New Data Based on a Subset of Grand Tour Data
There is rich information about meetings, exchanges of goods and services, and scandalous activities within the entries. If the students want to generate new entities and attributes, they will most likely be developing new schema as well to sit on top of the base Grand Tour schema. We will want to be able to track the new schema, export the new schema and let students share and compare so that they might revise and collaborate on those schema (or not). The outcome for the student is not only the new knowledge generated through the process, but the data added and the schema devised to make sense of the information.

###3. Generating a New Data Set

In this case, all views are all blank. Creating a new node in the Graph View or a new object in the Data View will populate the other two views. An unspecified entity type will appear gray in the Palette, faint in the Data View, and provisional (light or dotted border?) in the Graph View.  

**Starting with Grand Tour Schema**  
If a new data set is to be integrated into or verified against the Grand Tour data, start with a base Grand Tour schema which specifies existing entity types and attributes. These entity types will be options made available through the Data View or the Graph view when creating a new entity. The new entity will be pre-populated with place-holders for attributes for that entity type that exist in the Grand Tour schema.


###4. Integrating a New Data Set with Grand Tour Data
**With data based on Grand Tour schema**  
We need a workflow for contributing data to the larger data set. If the schema used is the Grand Tour schema, without any additions, we can consider the work as curation, meaning fixing errors or enriching the data set.

**With data created without or in addition to the Grand Tour schema**  
Provide the ability to map a student's schema to an existing schema (like the Grand Tour).



##Other

* We will want a view that show all of the other entity types connected to a given entity and how many. How many places are associated with James Gandy? How many letters? How many trips? How many publications?
* Tracking user-defined layouts.
* Track edits to replay and undo.
* Filter entities by date: Which have time and which do not? What date scale? Use a timeline to distribute values and for filtering.

