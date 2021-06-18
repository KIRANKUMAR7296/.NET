<p align=right><a href='https://github.com/KIRANKUMAR7296/SQL'>Navigate to SQL</a></p>

# C#

### C# Basic Concepts and Object Oriented Programming Concepts

---

### Can we use Multiple web.config file ? : `Yes`

- We have one Main Configuration File : `Web.Config`
- Then we have two more Configuration Files : `App.Config` and `Database.Config`
- `App.Config` :  Here we Define all the Application Level Settings ( Protocol, Request, Response )
- `Database.Config` : Here we Define all the Database Level Settings ( Data Source, Password )

```c#
<appSettings configSource="app.config">
</appSettings>
<connectionStrings configSource="database.config">
</connectionStrings>
```


