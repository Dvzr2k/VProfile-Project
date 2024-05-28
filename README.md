# VProfile-Project
A VProfile project setup (local), this project utilizes Vagrant to configure and provision a multi-machine infrastructure that supports a web application developed by hkhcoder. The infrastructure includes servers for MySQL, Memcached, RabbitMQ, Tomcat, and Nginx, all connected within a private network.

![image](https://github.com/Dvzr2k/VProfile-Project/assets/129244345/e9702fb9-f729-4a66-a1b8-06b8c5fadf92)

![image](https://github.com/Dvzr2k/VProfile-Project/assets/129244345/570611d4-220b-4768-8b53-52b1063ab46e)

![image](https://github.com/Dvzr2k/VProfile-Project/assets/129244345/66447c6f-cf02-4f9f-8c6f-c9afe2d4fe21)

![image](https://github.com/Dvzr2k/VProfile-Project/assets/129244345/22b30833-a26d-4580-9290-3cba5bd8d59e)

![image](https://github.com/Dvzr2k/VProfile-Project/assets/129244345/faae4308-8450-46d6-9613-0573b3eb09ee)


![image](https://github.com/Dvzr2k/VProfile-Project/assets/129244345/c0f9f30d-30be-4f05-96f7-3284f65232d1)
(RabbitMQ dummy service)

## Infrastructure Architecture

![vprofile](https://github.com/Dvzr2k/VProfile-Project/assets/129244345/a9c26039-f14d-404a-ad5d-9133c9b65faf)


The infrastructure is composed of the following machines:

1. **Database (MySQL)**:
   - **Name**: db01
   - **IP**: 192.168.56.25
   - **Operating System**: CentOS Stream 9
   - **Provisioning Script**: mysql.sh

2. **Memcached**:
   - **Name**: mc01
   - **IP**: 192.168.56.24
   - **Operating System**: CentOS Stream 9
   - **Provisioning Script**: memcache.sh

3. **RabbitMQ**:
   - **Name**: rmq01
   - **IP**: 192.168.56.23
   - **Operating System**: CentOS Stream 9
   - **Provisioning Script**: rabbitmq.sh

4. **Application Server (Tomcat)**:
   - **Name**: app01
   - **IP**: 192.168.56.22
   - **Operating System**: CentOS Stream 9
   - **Provisioning Script**: tomcat.sh

5. **Web Server (Nginx)**:
   - **Name**: web01
   - **IP**: 192.168.56.21
   - **Operating System**: Ubuntu 22.04 (Jammy Jellyfish)
   - **Provisioning Script**: nginx.sh
## Infrastructure Technologies
![image](https://github.com/Dvzr2k/VProfile-Project/assets/129244345/f9bc7a7d-02ad-4fd5-8f6a-61ee393e6928)

## Usage

1. Clone this repository to your local machine.
   ```sh
   git clone https://github.com/Dvzr2k/VProfile-Project.git
2. Run the following commands to create and configure the virtual machine.
   ```sh
   cd VProfile-Project-main
   vagrant up
   
3. Access the assigned IP address of the nginx virtual machine
   ![image](https://github.com/Dvzr2k/VProfile-Project/assets/129244345/6aca2fbf-41d6-4b54-9c9c-9e2f3cb0a37e)
   - Admin user: admin_vp
   - Admin password admin_vp

   

Enjoy developing!
