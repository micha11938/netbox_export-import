# netbox_export-import
In this file I show how to import data into netbox with the export / import feature of netbox.

https://github.com/netbox-community/netbox

Maybe this could save other people a bit of time because it's quite a bit of work before the data is ready for importing into netbox. And besides that I wonder if there is a quicker way to do this but for me this works.
What I did was export data from a running netbox application in Docker (I have a few running for test purposes) and after formatting the data in several steps, I imported the data into a running  production environment. 

But before you can import the data quite a lot of formatting needs to be done first because you can't import the exportfile without adapting the file to the prescribed netbox options format. 

Step 1: In netbox export data to csv file (my example 'Racks')

Step 2. Import data into excel  

Step 3. Convert data to netbox import format columns
(https://www.exceldemy.com/split-column-in-excel-by-comma/) Each comma in the export file, corresponds with an emtpy column.

Step 4. Export excel file to csv file 

Step 5. Open file with Sublime Text application 

Step 6. Reformat the CSV file to meet the demands of the netbox Fieldoptions import format. This is de Fieldoptions format for 'racks'. Site, regions, rackroles etc. have different Fieldoption formats.

Step 7. Import the data file into netbox and even then, mostly you will have to correct quite a few errors because the data nextbox exported mostly does not match with the demands of netbox. 

  

 
