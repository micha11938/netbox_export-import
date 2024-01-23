# netbox_export-import
In this file I show how I import data in netbox with the export / import feature. 

Maybe this could save other people a bit of time because it's quite a bit of work before the data is ready for importing in netbox. And besides that I wonder if there is a quicker way to do this. 
What I did was export data from a running netbox application in Docker (I have a few running for test purposes) and after formatting the data in several steps imported the data in a running acceptation and production environment.  
But before I can import the data quite a lot of formatting needs to be done. 

Step 1: In netbox export data to csv file (my example 'Racks')

Step 2. import data in excel  

Step 3. convert data to collum's  

Step 4. reformat the collums to netbox import format 

Step 5. export excel file to csv file 

Step 6. open file with sublime text application 

Step 7. reformat CSV file to meet the demands of the netbox import format. 

Step 8. import the data file in netbox and even then, mostly you will have to correct quite a few errors because the data nextbox exported mostly does not match with the demands of netbox. 

  

 
