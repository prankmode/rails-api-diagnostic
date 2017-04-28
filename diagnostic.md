# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
To implement the logic and to manage a persistance layer (database).
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
the model
```

Which layer in the MVC pattern communicates with the model?

```md
the controller
```

Why don't we use views in our interpretation of the MVC pattern?

```md
i have no idea - because we are going to use a client to do it and use rails as "just" an API?
```

What does C.R.U.D stand for?

```md
create/read/update/destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
controller
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
#create, #index, #show, #update, #destroy
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
-  the URL is sent to the router
-  the router decides which controller#method to send it to -> #show/:id
-  the controller needs data so it calls the model
-  the model generates the information, often by interacting with the database
-  the model returns the information to the controller
-  the controller sends it to the view for massaging
-  the view returns it to the web server
```

What is the command to generate a new rails-api app?

```bash
rails new <app_name>
```

What is the command to start an instance of a rails server?

```bash
rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
rails db:drop db:create db:migrate db:seed
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
rails generate model Pet name:string age:integer
```
