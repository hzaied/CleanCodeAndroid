# CleanCodeAndroid
This is a simple application that uses the clean code architecture.

Clean architecture
-----------------
![Clean code overview](https://github.com/android10/Sample-Data/blob/master/Android-CleanArchitecture/clean_architecture.png)

Architectural approach
-----------------
![Clean code approach](https://github.com/android10/Sample-Data/blob/master/Android-CleanArchitecture/clean_architecture_layers.png)

Block Diagram
-----------------
```java
                    Domain Layer               				   Data Layer
              ———————————————————————               —————————————————————————————
       ——>  |  ———  Interactor        |       ———> |	   Network	      	     |
      |	    | |			              |      |     |	    - Rest Apis	         |
      |	    |  ———> Executor          |      |     |                             |
      |	    |	    Repository   ———— | ——————————>|	   Storage  	   	     |
      |	    |	    Model             |            |	    - Content Providers  |
      |	    |	                      |            |	    - Database	         |
      |	      ———————————————————————               —————————————————————————————
      |
      | (Presenters calling interactors)
      |
      |
      |	          Presentation Layer
      |	     ————————————————————————————
      |	    |     UI   ————————————————— | ——
      |	    |       - Activities	     |   |
      |	    |       - Fragments	         |   | (UI calling the presenters)
      |	    |       - Adapters           |   |
      |	    |       - Views              |   |
       ————	|———— Presenters <———————————|———
             ————————————————————————————
```

TODO
-----------------
Need to add more clarification and code commenting to the code.
