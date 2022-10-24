# DOSP_Project3



## Team Members:
Pravallika Maddukuri- UFID : 5980-7015<br/>
Sai Siddharth Upadhyayula - UFID : 7459-9449<br/>

## Description
This project's goal is to implement the Chord protocol using overlay networks that can deliver services. This project uses Erlang and the Actor Model to illustrate the value of the Chord protocol.   

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
