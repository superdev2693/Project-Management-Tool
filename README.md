# Easy Project Management Tool

Easy project management tool is a desktop application made with Java and Javafx which enables you to manage your personal/office projects. You can add serveral projects & project’s tasks with milestone which will help you to complete the project successfully.

You can find how to use the tool [here](https://www.youtube.com/watch?v=W6fC6OQOjd0)

### How to build this tool in your local environment ?
This project is made using Intellij IDEA. So, I would **recommand** you to build this project using Intellij IDEA. 
1. Install Intellij IDEA from [here](https://www.jetbrains.com/idea/) if you don't already have it installed. You can install Community Edition. But if you are a student you can get the Ultimate Edition for free submitting your student identity info.
2. Fork & clone / download the source code of this repository in your PC.
3. We have stored information about different projects in a MySQL Database. You need the create a database with following 3 Tables, columns with mentioned datatypes. If you are using the Ultimate Edition of Intellij IDEA, you can create the database inside the IDE. If you are a Community Edition user, you can make the database with [sequel pro](https://www.sequelpro.com/) / [MAMP](https://www.mamp.info/en/downloads/)  

    Table name    | Column Name (String)   |  Column Name (String)
    ------------- | -------------  | ------------
    user          | ```username```   |  ```password```

    Table name    | Column Name (int)|  Column Name (String)| Column Name (Date) | Column Name (Date) | Column Name (String)
    ------------- | -------------  | -------------       | ------------        | ------------    | ------------
    project_info  | ```id```       |  ```project_name``` | ```start_date```    | ```end_date```  | ```estimated_time```


    Table name    | Column Name (int)|  Column Name (String)| Column Name (String) | Column Name (Date) | Column Name (Date) | Column Name (String)  | Column Name (String) | Column Name (String) | Column Name (String)  
    ------------- | -------------    | -------------        | ------------- | ------------       | ------------    | ------------ |---------- | ----------- | -------------
    project_task  | ```project_id``` |  ```task_name```     | ```time``` | ```task_start_date```   | ```task_end_date```  | ```progress``` | ```color``` |   ```dependency```  | ```assigned``` 
4. Config the database with application. You may need to edit [```Connnect.java```](https://github.com/atiqueahmedziad/Easy-Project-Management-Tool/blob/master/src/App/Connect.java) with your database name, user and password.
5. In ```User``` Table, make a row with ```username``` and ```password```. You will use the username and password for login authentication.
