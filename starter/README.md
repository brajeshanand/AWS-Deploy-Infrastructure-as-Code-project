# CD12352 - Infrastructure as Code Project Solution
# Brajesh Anand
## Infrastructure diagram
Below is the Infrastructure diagram that depicts the complete solution of the project created for Udagram webapp
<img width="2002" alt="udacity_udagram_network" src="https://github.com/user-attachments/assets/c1c76cc2-5da6-4aed-9431-9993ec4194b9">


## Spin up instructions
1. Open Visual Studio Code
2. Clone the branch at /workspace directory
3. Go to

   /workspace/AWS-Deploy-Infrastructure-as-Code-project-1/starter
4. To create the network stack, run the below command

   sh ./stack_scripts/create_stack.sh udagram-iac network.yml network-parameters.json
5. To create the Webapp stack, run the below command

   sh ./stack_scripts/create_stack.sh udagram-webapp udagram.yml udagram-parameters.json

Outputs
1. To verify the output of each stack, go to the Resources tab of both the stacks and verify the resources that are created.
2. Final output i.e. Udagram app can be checked at below URL.
 
   [udacit-webap-ecjwwhxvnjgp-2106369611.us-east-1.elb.amazonaws.com](http://udacit-webap-ecjwwhxvnjgp-2106369611.us-east-1.elb.amazonaws.com)
3. Below is the screenshot of the udagram webapp:
   <img width="622" alt="image" src="https://github.com/user-attachments/assets/2957ca5e-30c8-400f-8533-d8d2ac038565">



## Tear down instructions

1. Delete the stack using below command

   sh ./stack_scripts/delete_stack.sh udagram-webapp

2. Delete the network stack using below command

   sh ./stack_scripts/delete_stack.sh udagram-iac
