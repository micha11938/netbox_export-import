# netbox_export-import
In this file I show how to import data in netbox with the export / import feature. 

Maybe this could save other people a bit of time because it's quite a bit of work before the data is ready for importing in netbox. And besides that I wonder if there is a quicker way to do this but for me this works.
What I did was export data from a running netbox application in Docker (I have a few running for test purposes) and after formatting the data in several steps, I imported the data in a running  production environment. 

But before you can import the data quite a lot of formatting needs to be done first because you can't import the exportfile without adapting the file to the prescribed netbox options format. 

Step 1: In netbox export data to csv file (my example 'Racks')

Step 2. import data in excel  

Step 3. convert data to netbox import format  collum's
(https://www.howtogeek.com/407217/how-to-use-text-to-columns-like-an-excel-pro/#text-to-columns-with-delimited-text)In step 2 select 'Comma'. Each comma corresponds with an emtpy collumn.

Step 4. export excel file to csv file 

Step 5. open file with sublime text application 

Step 6. reformat CSV file to meet the demands of the netbox Fieldoptions import format. This is de Fieldoptios format for 'racks'. Site, regions, rackroles etc. do have different Fieldoption formats.

Step 7. import the data file in netbox and even then, mostly you will have to correct quite a few errors because the data nextbox exported mostly does not match with the demands of netbox. 

  

 
