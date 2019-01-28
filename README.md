# collaboration_visualizer
a simple tool to visualize academic collaborations on a world map


includes: collaboration_visualizer jupyter notebook and data created during the IDIES/UofT Visualization Hackathon - Winter 2019

The idea was to create a simple tool to visualize academic collaborations on a world map, by taking author and affiliation lists from scientific papers, matching the authors to their home institutions, getting the location (latitude and longitude) of these institutions using geocoder, and showing them on an interactive map - where clicking on the institution marker (sized by number of authors) shows you a list of everyone there, clicking on different collaborations turns those markers on off, etc..

Scraping authors and affialiations from a .pdf was harder than I'd hoped, so for now the author block from the pdf needs to copied and pasted to a string authors="""author string""", and the affialiation block from the pdf needs to copied and pasted to a string affiliations="""affiliations string""". Given this, I tried to deal with the strings in a way where the authors and institution strings don't need to be 
modified by hand toooo much... Copying and pasting from modern MNRAS articles at least works well

REQUIREMENTS:
1.) folium
2.) geocoder (or lat long already in a list)