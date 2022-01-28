
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
       
        # how to restore the data base
    
    
       source /home/pandi/pandiya.sql
       
       
    # how to install webserver apache2 in ubuntu
    
         sudo apt update
         
         sudo apt install apache2
         
         sudo systemctl status apache2

    #  how to stop,start,re-start apache2 
    
          sudo systemctl stop apache2
          
          sudo systemctl start apache2
          
          sudo systemctl restart apache2
          
   # how to remove the apache2 server
   
           sudo apt remove apache2
           
           
   # how to check port listen or not in mysql   
   
   
         netstat -tulpn | grep 3306     (mysql port3306)


    # how to check port listen or not  in apache2
    
    
          netstat -tulpn | grep 80       (apache2 port 800
          
          
    # how to check howmany potrs on ur system
    
    
           netstst -tulpn 


           
           
    # how to copy the file in one server to another server
    
    
           sudo scp pandi.txt ai@192.168.0.101:/home/ai 
           
            here pandi.txt is my system txtfile
            ai is another server user name
            192.168.0.101 is another server ip adress
            /home/ai is ai user home directory is copied
            
            
    # how to copy the another server file into my my server
    
    
          sudo scp  ai@192.168.0.101:/home/ai/c.txt /home/pandi  

           here c.txt is ai user file so c.txt copy to home directory of pandi
    
    
        
    
    
    
            
    
    
          

           
           
          

         

         
            
