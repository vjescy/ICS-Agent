This is the source code for ICSAgent that scans ICSHoneypot in the following way

1. Check if the HMI is available
2. Check if can login using default credentials
3. Check if all the Datapoints are available
4. Read the level of water in 3 tanks, wait 5 seconds, Read the level once again and calculate the delta (difference between outputs)

If all 3 deltas equal to 0, that is, there is no activity in the system or any of 1-3 fails the agent sends message to telegram bot

# Examples of error messages

1. HMI dead

   
  ![obraz](https://github.com/user-attachments/assets/6aa07276-88f4-470b-9ae0-f9c08517fb15)

  
2. Cannot login

   
   ![obraz](https://github.com/user-attachments/assets/4d3ed4ba-c20d-41a1-9ab1-4a3cc014a428)
   
3. Missing Datapoints

   
   ![obraz](https://github.com/user-attachments/assets/63c9dcde-d78c-4144-a323-c3a083cbf48b)
   
4. System halted/crashed/not working as expected

   
 ![obraz](https://github.com/user-attachments/assets/d1675991-7f21-4e5e-b990-83b2525d0b1f)





  
