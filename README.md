# AWS_NAT_INSTANCE_TUTORIAL
This project shows how to create an AWS NAT Instance and connect to the internet from a private subnet via a Jump-box linked with the NAT_INSTANCE

## STEP 1
  * Create a VPC and give it an appropriate IP Range e.g 10.0.0.0/16
  <img src = "./CreateVPC_1.JPG"/>

## STEP 2
  * Create Two Subnets 
    * One Public Subnet 
     <img src = "./CreatePublicSubnet.JPG"/>
     
    * One Private Subnet
     <img src = "./CreatePrivateSubnet.JPG"/>
    
## STEP 3 
  * Create an Internet Gateway through which your public subnet will access the internet
     <img src = "./CREATE_InternetGateway.JPG"/>
     * On creation of the Internet Gateway, you will see it detached like this:
      <img src = "./InitialStateOfYourIGW.JPG"/>
      
     * Click on Actions and attach your Internet Gateway to the VPC you earlier created
      <img src = "./Attach_YourIGW_To_VPC.JPG"/>
     
