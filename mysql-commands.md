 # how to install mysql server in ubuntu
 
    sudo apt update
    
    sudo apt install mysql-servers
    
    sudo systemctl status mysql
    
    sudo mysql_secure_installation

 # how to uninstall mysql in ubuntu
 
  sudo systemctl stop mysql

  sudo apt-get purge mysql-server mysql-client mysql-common mysql-server-core-* mysql-client-core-*

  sudo rm -rf /etc/mysql /var/lib/mysql
  
  sudo apt autoremove
  
  sudo apt autoclean


# how to login mysql root user

    mysql -u root -p
    
    
 # how to login mysql normal user
 
 
    mysql -u pandiyan -p
    
    

# creat user in mysql database


    CREATE USER 'pandiyan'@'localhost' IDENTIFIED BY 'Pandi@12345';

    GRANT ALL PRIVILEGES ON * . * TO 'pandiyan'@'localhost';


    FLUSH PRIVILEGES;
    
    
 
# how to  view table data 

      SELECT * From pandi ;  
      
  # how to change the database  
  
       use Sanjana;     
       
  # how to create the table      
       
       CREATE  TABLE  pandi  (Memberid int , MemberName varchar(255) , MemeberAge  int);
       
  # how to delete the table
  
  
         DROP Table pandi;
         
         
   # how to create database in mysql
     
         create database Sanjana;
         
   # how to delete database 
     
     
       DROP DATABASE Sanjana;
       
   # how to insert to data in tables
    
    
       INSERT INTO pandi VALUES (1, 'pandi', 30);

   # how to view the batabase

         show Sanjana;
         
         
   # how to delete one record from the table
    
    
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
    
    
          netstat -tulpn | grep 80       (apache2 port 80
          
          
   # how to check howmany potrs on ur system
    
    
           netstst -tulpn 


           
   # how to copy the file in one server to remote server
    
    
           sudo scp pandi.txt ai@192.168.0.101:/home/ai 
           
            here pandi.txt is my system txtfile
            ai is another server user name
            192.168.0.101 is another server ip adress
            /home/ai is ai user home directory is copied
            
            
  # how to copy the remote server file into  my server
    
    
        sudo scp  ai@192.168.0.101:/home/ai/c.txt /home/pandi  

         here c.txt is ai user file so c.txt copy to home directory of pandi
     
           
   # how to take ssh in remote server   
    
    
          sudo ssh ai@192.168.0.101
          
          ai is romote server name
           192.168.0.101 is remote server ip adress
           
           
   # How to stop the ssh server
   
      sudo service ssh stop
      
      sudo systemctl disable sshd.service
           
           
   # how to find the ip,subnetmask,getway,dns
   
   
        nmcli dev show wlp4s0 | grep -i ip4

             wlp4so is room wifi connection  
    
        
    
    
        
    
    
        
    
    
    
            
    
    
          

           
           
          

         

         
            
