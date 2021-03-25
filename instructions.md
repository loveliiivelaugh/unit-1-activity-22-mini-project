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

  6. Wrote out an external style sheet. ./assets/css/style.css

```
/*** Table of Contents ***

  1. Global Styling
    - text -- #4F4846

  2. Navbar
    - #266150

  3. Main section
    - #504846

  4. Contact section
    - #E8CEBF
    .btn -- #4F4846
*/


/* Global Styling */
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

body {
  position: relative;
  height: 100vh;
  width: 100%;
  color: #4F4846;
  font-family: Arial, Helvetica, sans-serif;
}

/* Navbar */
nav {
  background-color: #266150;
  width: 100%;
  margin: 0 0 20px 0;
  float: right;
  text-align: right;
  border-bottom: 8px #DDAF94 solid;
}

nav ul {
  display: flex;
  float:right;
}

nav ul li {
  list-style-type: none;
  text-decoration: none;
  color: #fff;
  margin: 20px 20px;
}

/* Main Section */
#main {
  width: 100%;
  margin: auto;
  text-align: center;
  top: 50%;
  display: relative;
}

#main h1 {
  margin: 10px;
}

#main p {
  margin: 20px;
}

.outer-most-box {
  height:315px;
  width: 315px;
  margin: auto;
  background-color: #504846;
  z-index: -2;
  text-align: center;
  top: 50%;
  display: flex;
}

.outer-box {
  height: 275px;
  width: 275px;
  margin: auto;
  border: 9px solid #E8CEBF;
  text-align: center;
  top: 50%;
  display: flex;
}

.middle-box {
  height: 225px;
  width: 225px;
  margin: auto;
  border: 8px solid #266150;
  top: 50%;
  display: flex;
}

.inner-box {
  height: 175px;
  width: 175px;
  margin: auto;
  border: 7px solid #DDAF94;
  top: 50%;
  display: flex;
}

.inner-most-box {
  height: auto;
  width: auto;
  margin: auto;
  border: 4px solid #444;
  top: 50%;
  display: flex;
}

.inner-most-box h2 {
  color: #E9CEBD;
  font-weight: 3000;
}

/* Contact Section */
#contact {
  position: absolute;
  bottom: 0;
  width: 100%;
  border-top: 2px solid #DDAF94;
  background-color: #E8CEBF;
  text-align: center;
  padding: 20px;
}

#contact h3 {
  margin: 10px;
}

form {
  border: 4px solid tan;
  border-radius: 20px;
  padding: 10px 20px;
  width: 40%;
  margin: auto;
}

.textfield {
  width: 70%;
  margin: 5px 0 0 0;
}

.btn {
  padding: 10px 40px;
  background-color: #4F4846;
  color: #fff;
}


```

7. Finshed. Tada!

![Finished!](/assets/screenshot-finished.png)