<p align=right><a href='https://github.com/KIRANKUMAR7296/SQL'>Navigate to SQL</a></p>

# C#

`C#` and `OOP` Concepts.

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


