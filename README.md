## jenkinsfiles
  A Jenkinsfile is a text file that contains the definition of a Jenkins pipeline and is used to automate the process of building, testing, and deploying applications. It is written using the Groovy programming language and can be created in two types: Declarative Pipeline and Scripted Pipeline.

  **1. Declarative Pipeline-**
   Declarative Pipeline is a more modern and user-friendly way to write Jenkins pipelines. It provides a structured and predefined syntax, making it easier to understand and maintain.

  **2. Scripted Pipeline-**
   Scripted Pipeline is more flexible and provides more control over the pipeline, but it requires a deeper understanding of Groovy.

  **Key Concepts**
  
    Agent:-Specifies where the pipeline or a specific stage will run. It can be a specific node, any available node, or a Docker container.
    Stages:- Defines different stages of the pipeline, such as Build, Test, and Deploy. Each stage can have multiple steps.
    Steps:- The individual tasks that are executed within a stage. These can include shell commands, invoking other tools, or performing specific Jenkins actions.
    Post Actions:- Defines actions that should be executed after the pipeline runs, such as cleaning up resources, sending notifications, or archiving results.

  **Benefits of Using Jenkinsfiles**

    Version Control:- Jenkinsfiles can be stored in the same repository as the source code, allowing the pipeline definition to be versioned and managed alongside the code.
    Code Review:- Changes to the Jenkinsfile can be reviewed through the same processes as code changes, ensuring quality and consistency.
    Reusability:- Common pipeline patterns can be reused across multiple projects, reducing duplication and simplifying maintenance.
