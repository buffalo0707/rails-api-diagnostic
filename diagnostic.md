# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
The backend allows multiple users to interact with a site and its data at once. It also stores data so that users can save/retrieve
things between sessions
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
The Model
```

Which layer in the MVC pattern communicates with the model?

```md
The Controller
```

Why don't we use views in our interpretation of the MVC pattern?

```md
Because views are handled in the client
```

What does C.R.U.D stand for?

```md
Create, Read, Update, Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
The Model
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
GET, PUT, PATCH, POST, DELETE
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
The client sends a GET request for '/people/1' to the server. The people controller on the server asks the People model to show the Person with ID 1. The Person model retrieves the data from the DB and presents it back to the client as a JSON string
```

What is the command to generate a new rails-api app?

```bash
gem install rails
```

What is the command to start an instance of a rails server?

```bash
bin/rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
-bin/rake db:drop
-bin/rake db:create
-bin/rake db:migrate
-bin/rake db:seed
-bin/rake db:examples
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bin/rails generate scaffold pet name:string age:integer
```
