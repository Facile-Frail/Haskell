# Haskell
### ***Installing Haskell (Linux)***
- **Check os details**

  ```lsb_release -a```

- **To install curl if you haven't already**

  ```sudo apt install curl```

- **To install haskell stack**

  ```curl -sSL https://get.haskellstack.org/ | sh```

<br><br>

### ***Getting it running***
- **Check if stack is installed**

  ```which stack```

- **Check stack version**

  ```stack --version```

- **Set your stack up (This is a one time process)**

  ```stack setup```

<br><br>

### ***Running a haskell file***
- **Be in the directory of your haskell file and run the runghc command**

  ```stack runghc <fileName>```

<br><br>

### ***Making a Project***
- **Be in the directory you want to create a project**

  ```stack new <projectName> <templateName(if any)> <resolver name(for a specific resolver)>```

- **As a beginner, use....**

  ```stack new <projectName>```

- ```cd <projectName>```

- **Build your stack**

  ```stack build```

  - **If the above command gives error and says stack is not initialised**

    ```stack init```

    ```stack build```

  This command makes an executable for your project and the path of this executable is given in the terminal after you run the ```stack build``` command

- **Run the executable**
    
    If you used the *simple* template, the name of your project's executable will be names as the project name itself.

    If any template is not used , the name of the executable is of the form ```<projectName-exe>```

  ```stack exec <projectName>```

  You can also run the executable manually

  ```<pathOfTheExecutable>/<nameOfTheExectuable>```