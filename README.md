### EXPERIMENT -07 CONFIGURING NETWORK SERVER FOR CONNECTING GATEWAY AND END NODE 
 
## Aim: 
To  configure the Network server and end device for transferring data on the network
## Components required: 
End node stm 32 development kit , Dragino LPS8, Network server 

## Theory :
When working with sensitive applications or files, saving progress on your local device is a start, but what if you lose access to your device? Network servers address this problem by hosting the files and programs most pertinent to the network and enabling access for consistent, real-time use. 

As a result, personnel or network clients can instantly access important data or tools while also facilitating collaboration between users. Multiple users can make changes to the same program or document for continued development over the course of a project. Via a secure login, remote users can connect to the home network.
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/59db9b76-ddd5-4d6a-9075-8db233f5e479)


In the above graphic, the circle represents an organization network where a network server facilitates collaboration and file sharing between network clients (devices).

 The role of a network server, then, is to provide users with a set of services and access to resources on the network. These features include:

Permissioned access and log-ins for network users Gateway access to the Internet for an organization Centralized location for network resources  Shared access to devices on the network like a printer or a scanner Hosts multi-user apps like email servers, web applications, or CRM

## Procedure :

 1. login to the network server using login link  https://iot.saveetha.in/
 2. Click on the nework server as shown blow
    
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/1bd434ca-1426-4102-8384-94473483543e)
 3. Click on the add gateway 
 
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/47c2e08d-6598-4437-8b07-f213d6f3b8ac)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/e62ff028-99bc-485e-9808-fbb6e124f8b2)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/a2e3ae58-6402-49e8-8f96-679059c1842c)
4. Click on the lora options , lora - frequency plan 

5. Click on channels and create a new channel after which you can add a new end device
   
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/1fb72be5-e48d-4cde-a329-0cfb0d29070f)

6. Add the attributes in the end device as  shown below 

 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/00bff30b-42fc-42d5-9540-285d270e41cb)
 
7.Using AT commands configure end device in serial port utility
AT Commands to set initially (Mandatory)
 AT+FDR // To do factory data reset
 AT+NJM=1 // To set OTAA mode
 AT+ADR=1 // To enable the ADR
 AT+TDC=600000 // To set the default sampling interval as 10 minutes
(Should not give below 5 minutes)
 AT+CLASS=C // To set class C
 AT+DEUI=XX XX XX XX XX XX XX XX // To set Device EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX // To set APP EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX //
To set APP Key
 ATZ // To take effective action on below settings (As like saving)



## OUTPUT 
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/23c688c9-22fe-4256-84c3-86cfe854f185" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/014339cb-3925-4afb-b123-5996ccf33404" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/9d35ffdd-325d-42cc-aaf2-00b8af3566cd" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/261b8bcf-6559-4ce5-b23b-cc5ed07d9bff" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/946c5f0f-e5b8-447c-ba4b-c3a23ec648f2" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/63504c7b-4b52-4917-ab8f-9dcf28583642" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/dd35902c-531f-4651-a395-1b97300c0c36" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/d15d6e91-0483-44d2-a513-82649bbc916e" />

<img width="1920" height="1080" alt="Screenshot (603)" src="https://github.com/user-attachments/assets/faa78d40-7212-4849-95f1-04d3d8ff5746" />

<img width="1920" height="1080" alt="Screenshot (595)" src="https://github.com/user-attachments/assets/165293ef-e4d5-48a2-836c-0a67a93715ba" />

<img width="1920" height="1080" alt="Screenshot (596)" src="https://github.com/user-attachments/assets/8762e237-6ced-4296-912a-df400dcc782e" />

<img width="1920" height="1080" alt="Screenshot (597)" src="https://github.com/user-attachments/assets/0316a964-8d10-48ff-93d3-4362b0f0be89" />

<img width="1920" height="1080" alt="Screenshot (598)" src="https://github.com/user-attachments/assets/ea456899-b6ff-43e4-869c-af39ee99ca84" />

<img width="1920" height="1080" alt="Screenshot (599)" src="https://github.com/user-attachments/assets/db25639e-564e-4686-94a9-d4868d293883" />

<img width="1920" height="1080" alt="Screenshot (600)" src="https://github.com/user-attachments/assets/32e898c1-2ab7-41d6-8bbe-b1b15325f4e3" />

<img width="1920" height="1080" alt="Screenshot (601)" src="https://github.com/user-attachments/assets/89a22248-4aa5-4be9-b82d-b778b2489cd0" />

<img width="1920" height="1080" alt="Screenshot (602)" src="https://github.com/user-attachments/assets/a84ccbcb-d72d-4efe-ad5b-22d6f19e4f19" />

<img width="1920" height="1080" alt="Screenshot (604)" src="https://github.com/user-attachments/assets/b46c4645-89c9-46dc-b3af-0d95d0d32a79" />


## Result: 

  The Network server and end device for transferring data on the network has been accomplished.
