---

layout: post
title:  "Palladio FAQ"
author: Mark Braude
date:   2014-04-29 11:34:22
category: palladio
published: false
tags: 
excerpt: ""
 
---

#Frequently Asked Questions

- [What is a Palladio Data Model?](##What is a Palladio Data Model?)  
- [Which data formats work with Palladio?](##Which data formats work with Palladio?)

					<li><a href="#faqdataformat">Which data formats work with Palladio?</a></li>
					<li><a href="#faqlightning">What does it mean if I see a Lightning Bolt icon and ‘Special Characters Found’ in one of my dimensions?</a>
					<li><a href="#faqmultiple">What is a Multiple Values Delimiter?</a></li>
					<li><a href="#faqsize">What are Size Points?</a></li>
					<li><a href="#faqtime">How do I get the most use out of the Timeline feature?</a></li>
					<li><a href="#faqdates">How should Dates be entered?</a></li>
					<li><a href="#faqcoord">How should Coordinates be entered?</a></li>
					<li><a href="#faqlabels">What do the labels (text, date, URL etc.) and numbers listed directly below my dimension represent?</a></li>
					<li><a href="#faqexport">I would like to export a Map visualization but you only allow .svg export for Graph visualizations. What should I do?</a></li>
					<li><a href="#faqgallery">What are some applications of the Gallery View?</a></li>
					<li><a href="#faqmap">How do I get the most out of Map view?</a></li>
					</ul>


##What is a Palladio Data Model?

					<p>Once you’ve uploaded your tabular data into the Palladio interface, you may refine it and save it as a Palladio Data Model to your desktop.  The Palladio Data Model is saved with the extension .json and includes the schema and structure required to visualize your data in Palladio. (Not just any json file will do.) Now, as you continue to use Palladio you can shorten the upload and refine stages by uploading your existing palladio.json file (The Palladio Data Model). Remember that if you make further changes to your data in the refine stage, you should re-export the Data Model to have a version that reflects your changes.</p>



##Which data formats work with Palladio?

					<p>Any collection of information that can be represented in a table format (in other words, any data you might enter into a spreadsheet program) will work with Palladio. Make sure that all data is represented by delimited-separated values. Palladio supports the following delimiters: commas, semicolons and tabs.</p>

					<p>Palladio works best with data that is uniform, consistent, and simple. Avoid notes and comments within your data, or any unnecessary diacritics.</p>

					<p>You can build your own tables and bring them into Palladio in three ways:</p>

					<ol>
					<li><p>By typing text into any word processing program (ie. textedit or MS Word) and then copying the contents into Palladio interface.</p></li>
					<li><p>By dragging any file format into the Palladio interface, for instance by dragging a .txt file from your work station and dropping into Palladio.</p></li>
					<li><p>By typing directly into the Palladio interface.</p></li>
					</ol>


					<p>If you plan to build your own table in Palladio:</p>

					<p>The first row in your data will be parsed as a header. This means that the first row in your data will indicate the name of the dimensions in the column below.</p>

					<p>So, a table column of people's names would have 'Names' as its first row and then dimensions, such as 'John Doe' and 'Jane Smith' in the rows below. Palladio cannot properly access and reference the different dimensions in your data unless you follow this format.</p>

					<p>Each column header must be unique from the other. Within a header name you may use letters, spaces, and numbers. Do not use any special alphanumeric characters, such as underscores '_' or dashes '-', as these will confuse Palladio.</p>

					<p>Examples of data:</p>

					<p><em>Correct</em>:</p>

					<p>First name, Last name, Age</p>

					<p>John, Doe, 28</p>

					<p>Jane, Smith, 35</p>

					<p><em>Incorrect</em> (missing header):</p>

					<p>John, Doe, 28</p>

					<p>Jane, Smith, 35</p>

					<p><em>Incorrect</em> (two headers with the same name):</p>

					<p>Name, Name, Age</p>

					<p>John, Doe, 28</p>

					<p>Jane, Smith, 35</p>

					<p><em>Incorrect</em> (special characters in the header):</p>

					<p>First_Name, Last-Name, Age</p>

					<p>John, Doe, 28</p>

					<p>Jane, Smith, 35</p>

					<h5>Other Data Issues</h5>

					<p>Note that empty rows in your data will be ignored by Palladio.</p>

					<p>Palladio does not work with unstructured data, such as one long string of text, but only with data that has been placed into some kind of table. The richest uses of Palladio comes from having several different related tables of information, however many users will start with just one single table.</p>



					<h4 name="faqlightning">What does it mean if I see a Lightning Bolt icon and ‘Special Characters Found’ in one of my dimensions?</h4>

					<p>This is Palladio’s way of telling you that there are non-standard alpha-numerical characters in your data. These special characters may either lead to errors, or (in the case of commas or semicolons used to separate values in a given dimension) these special characters may be of help for you to use advanced tools such as the Multiple-Values Delimiter.</p>


					<h4 name="faqmultiple">What is a Multiple Values Delimiter?</h4>

					<p>Your tabular data is made up of various dimensions (ie. individual cells in a spreadsheet). In some cases you may want to assign more than one value for a certain dimension. For instance, you may have a column describing someone's 'Position.' The column could be filled Princes, Popes, and Poets. But what if your Prince was also a Pope? In this case you could enter 'Prince, Pope' in one single cell of your table. Now, after you’ve uploaded the data into Palladio, you can parse that cell into two unique values. Here's how: In the Multiple Values Delimiter input box, enter the symbol you've used to separate your values, in this case, a comma that separated Pope and Prince. Now Palladio understands that this entry as two separate values.</p>



					<h4 name="faqsize">What are Size Points?</h4>

					<p>Toggling the Size Points function in the map view will change the sizes of your various dots on the map, depending on how frequently they appear in your dataset. So, for instance, if you had a table listing 30 Priests born in Rome and 1 Priest in Florence, and you have produced a map visualization that counts by Priests, the dot representing Rome in your map view will be significantly larger than the dot representing Florence.</p>


					<h4 name="faqtime">How do I get the most use out of the Timeline feature?</h4>

					<p>As you change the temporal period in your timeline view, the map will update to show data only from that period. You can zoom in to get as granular a view as you would like. One of the most exciting features of Palladio’s timeline is that it allows users to select more than one point on the timeline to show more than one period (ie. 1900-150) and 1970-200) view these simultaneously within a given visualization.</p>

					<p>Swiping within the Timeline view will allow you to zoom in to specific dates. The stacked bar and highlighting functions allow you to see the data in different ways as you hover.</p>


					<h4 name="faqdates">How should Dates be entered?</h4>

					<p>Dates should be entered in the following format Year-Month-Day (2014-01-01). Years must always be rendered as four digit integers. Thus years between 0 CE and 1000 CE should still be rendered as 0001 or 0999. Palladio does not yet handle years before 0 CE.</p>



					<h4 name="faqcoord">How should Coordinates be entered?</h4>

					<p>Coordinates information must be rendered as latitude and longitude, separated by a comma. For example: 41.95, 12.5.</p>

					<p>Visit the Scenario: Creating Data for a Simple Map in the Tutorials section for more information about creating and entering coordinates information.</p>


					<h4 name="faqlabels">What do the labels (text, date, URL etc.) and numbers listed directly below my dimension represent?</h4>

					<p>In the refine (non-visualization) view your data appears as table, with each column header represented as a unique dimension.</p>

					<p>For instance, Gender as the Dimension Name, with the label Text and number 2 listed below.</p>

					<p>In this case Gender is the header from one column of your data, Text is the data type recognized by Palladio (most data will be recognized as Text), and the number 2 represents the number of unique values in your data - in this case the data contains 2 values: Male and Female.</p>

					<p>Palladio will guess the type of data entered based on its attributes. Data will be recognized as either: Text, Number, Year or Date, Coordinates, URL.</p>

					<p>If Palladio ‘guesses’ your data incorrectly you can click on the dimension and in the dropdown menu labeled Data Type, change the type of data specified. The more accurately Palladio defines your data, the better the platform will work.</p>


					<h4 name="faqexport">I would like to export a Map visualization but you only allow .svg export for Graph visualizations. What should I do?</h4>

					<p>As Palladio Map Visualizations involve placing static coordinates data onto a separate map grid layer the full visualization cannot currently be exported as an svg. We recommended using ‘screen grabs’ as the best method, currently, for exporting map visualizations.</p>



					<h4 name="faqgallery">What are some applications of the Gallery View?</h4>

					<p>In the Gallery View you can display different kinds of data that cannot be visualized as maps or graphs.</p>

					<p>For instance, if in your data set you had a column in which you linked a list of people to URLs containing images of each person, you could then display these images in grid view.</p>

					<p>In this case, you would go to Grid View and click the ‘Image URL’ option. Palladio would then locate the dimension in which you’ve listed image URLs in your data.</p>


					<h4 name="faqmap">How do I get the most out of the Map view?</h4>

					<p>The default map view is a blank map. Note the settings panel to the right. You can hide the panel by clicking on the gear symbol. The + and - signs zoom the map in and out.
					The first step is to specify the type of map you'd like to see. To do so, choose from the menus within the settings panel. You can choose from two types of map views: 'Points' or 'Point to Point'. (Note that access to these functions will depend on the kinds of information you've uploaded. You wouldn't, for example, be able to use the 'Point to Point' function unless Palladio recognizes a dataset with more than one type of coordinates column, ie. 'Source City' and 'Destination City.')</p>

					<h5>‘Points’ map view</h5>

					<p>In the 'Points' map view, Palladio can map out a collection of unique locations, based on any coordinates data (longitude, lattitude) you've entered. For instance, if you uploaded a table listing all of the Popes in the last five hundred years, their individual cities of birth, and coordinates data for each of these cities, you might want to see a worldwide view of where Popes have been born in the last five hundred years.</p>

					<p>In Points view you can only select one dimension. If you toggle Size points, the sizes of each dot will relates to their frequency within your data. You can specify how you would like to count your data by using the Count By function. Note you can only count by unique tables uploaded in your data. Hovering over specific dots will display corresponding data. You can select which type of data to display on hovering, by using the Tooltip label.</p>

					<p>Below the 'Type of Map' menu is a second menu, 'Places.' This menu will be populated with any data for which there are coordinates, and the menu choices will be named for the headers of columns containing coordinates data. For instance, in our Popes dataset set, if the coordinates data in your original table is labeled 'Birth City Coordinates,' then you will be prompted to choose 'Birth City Coordinates' within the 'Places' menu. To see all of your Popes birthplace data on the map, you would select 'Birth Place Coordinates' in the 'Places' menu. Now the map will be populated with dots representing each individual value in your coordinates data.</p>

					<h5>‘Point-to-Point’ map view</h5>

					<p>The point to point view give us a node-link map. Here you will select two different dimensions (ie. source city and destination city) and see the links between various points.</p>

					<p>The arc of the link between two points represents the direction of the flow. Think of direction in a clockwise function.</p>

					<p>Now you can explore this Map data in various ways by using the Timeline and Facet Filter functions. You can also use the search bar to filter the data being visualized to accord with whatever parameters you wish, so long as your coordinates data corresponds in some way to whatever you've typed into the search bar. You can also isolate specific points on your map by clicking on them.</p>


              	<hr class="col-md-12">
              	<h2 id="opendesign">Open Design for Humanities Research</h2>
      			<p>Palladio is a work in progress. We will be releasing new versions throughout the year from January to December 2014. We want to make it useful for research and teaching and your feedback will help us get there. Share your questions and comments about how to improve Palladio and will respond directly by email.</p> 
                <p>Please email us at <a href="mailto:palladio@designhumanities.org">palladio@designhumanities.org</a> to share your experience.</p>
              
