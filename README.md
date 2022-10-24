# DOSP_Project3



## Team Members:
Pravallika Maddukuri- UFID : 5980-7015<br/>
Sai Siddharth Upadhyayula - UFID : 7459-9449<br/>

## Description
This project's goal is to implement the Chord protocol using overlay networks that can deliver services. This project uses Erlang and the Actor Model to illustrate the value of the Chord protocol.   

## Execution Steps - 

1. Create a node for the server using the command -

      erl -name pravallika@10.20.32.67

2. Compile the modules using the command -

      c(project_3). <br/>
      

3. To start the compiled program and enable the main module, use the command - 

      project_3:root(2,2)

      Here the first argument represents the number of nodes. The second argument represents the number of requests.


## Report Questions

1. What is working ? -<br/>
•	The chord rule executes perfectly.<br/>
•	Each individual node has a table with entries to and from the node known as the finger table.<br/>
•	Every node creates a unique key value for every request received.<br/>
•	Once all the individual computers are ready, we can perform a lookup for a key value on an arbitrary individual computer and if the lookup does not         match the current node, then the lookup can be transferred to the neighboring individual computers by making use of the log table.<br/>
•	The number of jumps increases for each key value once a search is successful.<br/>
•	Each individual computer responds to the requests received and returns the total jumps per lookup and stops.<br/>
•	Lastly, the mean of the total jumps per search in the chord setup is calculated.<br/>

Highest Working Node Screenshot:
<img width="958" alt="highest node" src="https://user-images.githubusercontent.com/116412716/197445068-7600bfa0-6f74-42d0-bdfc-4668a45738a4.png">


2.INPUT PROVIDED-<br/>
      Number of Nodes and Number Of Requests
      
3.OUTPUT -<br/>
      Average Hops = Total Hops / Total received requests

      The maximum chord setup size to be obtained is with 15,000 with mean jump value = 5.941.
      
4. FINDINGS
      The number of nodes is directly proportional to the mean hop size.
      The number of requests received is inversely proportional to the mean hop size. 
      
      Dataset Screenshot
      <img width="319" alt=" dataset screenshot" src="https://user-images.githubusercontent.com/116412716/197445099-32f934be-4f57-4ccf-a63f-24f3d40b79ae.png">

      Graph
      <img width="646" alt="graph" src="https://user-images.githubusercontent.com/116412716/197445118-6196aa4d-eb4d-43ca-a86f-9bbaf7db68a1.png">






