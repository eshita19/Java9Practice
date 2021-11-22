# Java9Practice

## Jshell
 - Interactive tool for learning Java programming language.
 - <img width="575" alt="Screenshot 2021-11-18 at 2 22 04 PM" src="https://user-images.githubusercontent.com/33754197/142382844-1fba7429-7720-4d8c-986c-4bcb06147c07.png">

## Java modules
  - Encapsulates code further by controlling the code exposed in project.
  - module-info.java => Module definition 
 ```
  module com.esh {
	exports com.esh;
	requires com.esh.module3;
}
```
 
## Jlink
  - Create custom JRE.
  ```
  $JAVA_HOME/bin/jlink	\
	--module-path $JAVA_HOME/jmods:out \
	--add-modules academy.learnprogramming.jokeapp \
	--launcher JOKER=academy.learnprogramming.jokeapp/academy.learnprogramming.jokeapp.Main 	\
	--output jre

  ```
