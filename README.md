# DOSP_Project3



## Team Members:
Uma Sai Sree Avula - UFID : 38554667<br/>
Bhanu Rekha Musuluri - UFID : 98477459<br/>

## Description
This project implements the gossip algorithm which is used for propagation of the data. There are actors in the model and each actor stores two variables s and w. Upon receiving the message from other neighbour actors, the variables get added up and upon sending the messages the values of variables are halved. Each time s/w value is calculated and we terminate the algorithm when the value of s/w doesn't change more than 10^-10 in 3 consecutive rounds. Hence this project is helpful in determining the convergence of gossip algorithm.   

## Execution Steps - 

1. Create a node for the server using the command -

      erl -name uavula@192.168.0.105

2. Compile the modules using the command -

      c(gossip). <br/>
      c(pushsum). <br/>
      c(topology). <br/>
      c(main). <br/>

3. To start the compiled program and enable the main module, use the command - 

      main:start(8192, "2D", "gossip").

      Here the first argument represents the number of workers. The second argument represents the type of topology. The third argument represents the name       of the algorithm.


## Report Questions

1. What is working ? -
