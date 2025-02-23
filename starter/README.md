# Infrastructure as Code Project Solution
# Brajesh Anand
## Infrastructure diagram
Below is the infrastructure diagram illustrating the end-to-end solution designed for the Udagram web application
<img width="2002" alt="Image" src="https://github.com/user-attachments/assets/29c1216a-985a-4b64-886e-e1964e6500fe" />


## Spin up instructions
1. Open Visual Studio Code
2. Clone the branch at /workspace directory
3. Go to

   /workspace/AWS-Deploy-Infrastructure-as-Code-project/starter
4. To create the network stack, run the below command

   sh ./stack_scripts/create_stack.sh UdacityNetwork network.yml network-parameters.json
   
   
   Note : wait for stack to come into CREATE_COMPLETE status

5. To create the Webapp stack, run the below command

   sh ./stack_scripts/create_stack.sh UdacityUdagram udagram.yml udagram-parameters.json

Outputs
1. To verify the output of each stack, go to the Resources tab of both the stacks and verify the resources that are created.

2. Final output i.e. Udagram app can be checked at below URL.
 
   [udacit-webap-ecjwwhxvnjgp-2106369611.us-east-1.elb.amazonaws.com](http://Udacit-WebAp-ecjWWhXvNjGp-2106369611.us-east-1.elb.amazonaws.com)

3. Below is the screenshot of the udagram webapp:
   <img width="953" alt="Image" src="https://github.com/user-attachments/assets/249c35e1-1b4f-4e4d-9f27-063ea08c614d" />



## Tear down instructions

1. Delete the stack using below command

   sh ./stack_scripts/delete_stack.sh UdacityUdagram

2. Delete the network stack using below command

   sh ./stack_scripts/delete_stack.sh UdacityNetwork
