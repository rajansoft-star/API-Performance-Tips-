# Simple API-Performance-Tips
This will covers only API performance related tips 

Performance tips

  * Code should be written in async 
  
  * SQL query Optimailiztion 
  
  * Needs Handle Proper Caching (use Redi cache,Meme Cache,Node cache)
  
  * Go session free approach becuase session story in in memory , if not possible atlest have minimum level of data in session
  
  * Use Logger to track bug information
   (Use Winston, Morgen, etc.,framework for Node Js , for .Net use Nlog ,Serilog ,MicrosoftExtenstion Logger,etc.,)
  
  * Use Run Parallel 
      Ensure parallel execution flow when requesting remote services, database calls, and file system access.
	  Parallelizing tasks will greatly reduce latency and minimize any blocking operations. Parallel operation means running multiple things at the same time.
    
	       Generally, Node.js does not technically execute these multiple tasks at the same time. What happens is that each task is pushed to an asynchronous 
	       event loop with no control of which task will finish before the other. If your execution needs to complete one or more tasks before the
         other please consider going asynchronous.Install async async.parallel(tasks, callback).
    
* Using the latest stable Node.js/Net or other framework  updates
* Use Load balancing Enviroment 
* Eliminate unused components of .js libraries or class library file from the code
* Removing unused lines of codes from the project
* Prioritize access to local variables
* Having a well-defined execution context
* Avoid global variables Declaration
