<p align=right><a href='https://github.com/KIRANKUMAR7296/SQL'>Navigate to SQL</a></p>

### What is MVC ?

- `MVC` : Model `Data` + View `UI` + Controller `Brain`
- Core concept is to separate the `business logic`, `user interface` and `data model` from each other.
- `Model` : A model extracts data from a database like `cloud`, `local storage`, `API's`
- `View` : View represents the `UI` of app, it shows the data model and takes inputs from the users.
- `Controller` : Consist of `business logics`, control and decide what will be displayed to user.
- `MVC` helps to make work easy, structured and organized.
- So if something is changed in one part of the project, it will not affect other parts of the project. 
- User interacts with `view` on which data is displayed and provide input with `controller` through `view`
- `Controller` is like brain it manipulates the data for user or take data from `model` to work.
- And after work is completed again it is provided back to `view` which shows desired data to users.

### Can we use Multiple web.config file ? : `Yes`

- We have one main configuration file : `Web.Config`
- Then we have two more configuration files : `App.Config` and `Database.Config`
- `App.Config` :  Here we define all the application level settings ( Protocol, Request, Response )
- `Database.Config` : Here we define all the database level settings ( Data Source, Password )

```c#
<appSettings configSource="app.config">
</appSettings>
<connectionStrings configSource="database.config">
</connectionStrings>
```

### `ASP.NET Full Stack Developer`

- `Front End` : `HTML`, `CSS`, `Bootstrap` (CSS library), `JavaScript` and `jQuery` (JavaScript library)
- `Back End` :  `C#` programming language
- `Framework` : `ASP.NET`
- `Database` :  `SQL`
 
### MVC `Authentication` ( Username and Password )

- A process to `ensure` and `confirm` a user’s identity.
- Whether user is registered or not to access particular data or web pages.
- A process to `validate` someone.

### MVC `Authorization` ( Permission )

- Determine whether the user has `access` to a particular resource or not.

`Authentication` happens first and then `Authorization` is determined.

### Authentication Types

1. `Forms` Authentication : Provide credentials through form ( Username and Password )
2. `Window` Authentication : `IIS` Authentication
3. `Password` Authentication : Centralized authentication service provided by Microsoft Autheticator.

