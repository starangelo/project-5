## CLIENT-SERVER ARCHITECTURE WITH MYSQL
Two ec2 instances were created for 'mysql-server' and 'mysql-client'.
EC2 instance for mysql-server.
![ec2_mysql-server](./img/1%20connect%20server%20ec2.png)
EC2 instance for mysql-client.
![ec2_mysql-client](./img/2%20connect%20client%20ec2.png)
Then mysql shell is installed for both server and client. 
mysql for server.
![mysql-server](./img/3%20install%20mysql%20server.png)
mysql for client.
![mysql-client](./img/4%20install%20mysql%20client.png)
On the security group of the mysql-server, the port 3306 is configured to allow access.
![port-3306](./img/5%20security%20group%20allows%20port%203306%20for%20server.png)
From the server terminal the bind-address was changed to 0.0.0.0 in order to give access to the client while connecting via TCP\IP.
![bind-address](./img/6%20To%20allow%20connection%20from%20remote%20host.png)
Mysql interface is connected to so as to make the neccessary configuration, create the user and grant the privilege in order for the client to be able to connect remotely.
![connect_server](./img/7%20connect%20to%20mysql%20server.png)
Mysql-client connects remotely using the mysql utilities. This shows that the client is connected to the mysql-server.
![connect_mysql_client](./img/8%20client%20connected%20to%20the%20mysql-server.png)
Below is a confirmation of the connection.
![confirmation](./img/9%20check%20to%20see%20that%20connection%20is%20successful.png)
