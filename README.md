# Unit 1 Activity 22 Mini Project

## Description

## Instructions

1. In the terminal.

`cd ~ && cd Desktop && cd classActivities && mkdir <your-project-title> && cd <your-project-title>`

- now that were into our new project directory.

`touch index.html && mkdir assets && cd assets && mkdir css && cd css && touch style.css && cd .. && mkdir images && cd ..`

- We'll use these two commands to initiate our project starting files and file structure.

2. Create a new repository in GitHub. Then enter the following in terminal, line by line.

```
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin <your-new-github-repo-url.git>
git push -u origin main
```

3. Check mock-up for project criteria. And start coding...

![Mock-up](/assets/screenshot.png)

#### index.html

4. Boilerplate code.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <title></title>
    <meta name="description" content="">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="./assets/css/style.css">
  </head>
  <body>

  </body>
</html>
```

5. First thing's first, lay out semantic HTML elements that correlate with the mock-up

```
<body>

  <!-- Navbar component -->
  <nav>
    <ul>
      <a href=""><li>Github</li></a>
      <a href=""><li>Portfolio</li></a>
      <a href=""><li>Contact</li></a>
    </ul>
  </nav>

  <!-- Main Section component -->
  <section>
    <h1>My New Website</h1>

    <div>
      <div>
        <div>
          <div>
            <h4>COMING SOON</h4>
          </div>
        </div>
      </div>
    </div>

    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
  </section>

  <!-- Contact Section component -->
  <section>
    <h3>Contact Me</h3>
    <form onsubmit="formHandler(data)">
      <div>
        <label>Name:</label>
        <input type="text" />
      </div>
      <div>
        <label>Email:</label>
        <input type="text" />
      </div>
      <div>
        <input type="submit" value="Send" />
      </div>
    </form>
  </section>

<!-- Added a little bonus script here to alert us when the form is submitted -->
  <script>
    const formHandler(event, data) {
      event.preventDefault();
      alert({
        message: "Congratulation's, form is submitted!",
        data: data
      })
    }
  </script>

  </body>
  ```

  6. Wrote out an internal style sheet to start gauging the way things are put.

```

    <!-- Nav Bar styling -->
    <style>
      * {
        box-sizing: border-box;
        padding: 0;
      }

      body {
        height: 100vh;
        width: 100%;
      }
      
      nav {
        background-color: olivedrab;
        width: 100%;
      }
      
      nav ul {
        display: flex;
      }
      
      nav ul li {
        list-style-type: none;
        text-decoration: none;
        color: #fff;
        margin: 20px 20px;
      }

      #main {
        height: 50vh;
        width: 100%;
        margin: auto;
        border-top: 3px #dbc solid;
        text-align: center;
      }

      .outer-most-box {
        height:400px;
        width: 400px;
        background-color: brown;
        z-index: -2;
      }

      .outer-box {
        height: 350px;
        width: 350px;
        border: 6px solid tan;
      }

      .middle-box {
        height: 300px;
        width: 300px;
        border: 5px solid green;
      }

      .inner-box {
        height: 250px;
        width: 250px;
        border: 4px solid tan;
      }

      .inner-most-box {
        height: auto;
        width: auto;
        border: 3px solid #222;
      }

      #contact {
        border-top: 1px solid tan;
        background-color: bisque;
        text-align: center;
        padding: 20px;
      }

      form {
        border: 4px solid tan;
        border-radius: 20px;
        padding: 10px 20px;
        width: 35%
      }

      .textfield {
        width: 300px;
        margin: 5px 0 0 0;
      }

      .btn {
        padding: 10px 40px;
        background-color: #333;
        color: #fff;
      }

    </style>
```

* *Far from perfect but things just need to be adjusted from here and it will be all set.*

![phase1](/assets/screenshot-phase1.png)