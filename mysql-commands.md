
# how to login mysql root user

    mysql -u root -p
    
    
 # how to login normal user
 
 
    mysql -u pandiyan -p
    
    

# mysql user creation 


    CREATE USER 'pandiyan'@'localhost' IDENTIFIED BY 'Pandi@12345';

    GRANT ALL PRIVILEGES ON * . * TO 'pandiyan'@'localhost';


    FLUSH PRIVILEGES;
    
    
 
# view table data 

      SELECT * From pandi ;  
      
  # how to change the database     
       use Sanjana;     
       
  # how to create the table      
       
       CREATE  TABLE  pandi  (Memberid int , MemberName varchar(255) , MemeberAge  int);
       
  # how to delete the table
  
  
         DROP Table pandi;
         
         
     # how to create database in my sql
     
         create database Sanjana;
         
     # how to delete database 
     
     
       DROP DATABASE Sanjana;  
    # how to insert to data in tables
    
    
       INSERT INTO pandi VALUES (1, 'pandi', 30);

       # how to view the batabase

         show Sanjana;
         
         
    # how to delete one record from thetable
    
    
         DELETE FROM pandi  WHERE Memberid=2;
         
         
    # how to delete total records in table 
    
    
        DELETE FROM pandi;
        
        
    # how to delete one colomn in table
    
       ALTER TABLE pandi DROP COLUMN Memberid;
       
    # how to install webserver apache2 in ubuntu
    
         sudo apt update
         
         sudo apt install apache2
         
         sudo systemctl status apache2

    # how to sto,start,re-start apache2 
    
          sudo systemctl stop apache2
          
          sudo systemctl start apache2
          
          sudo systemctl restart apache2
          
   # how to remove the apache2 server
   
           sudo apt remove apache2
           

         

         
            
