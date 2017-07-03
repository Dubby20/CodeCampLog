### Wednesday June 28th, 2017

* Learnt how to initialize Git repository
* Added my First Portfolio to my GitHub Account 

### Thursday June 29th, 2017

* Updated my Portfolio Website

## Friday June 30th, 2017

* Learnt how to style using Bootstrap
* Learnt how to create rows and columns using Bootstrap
* Used Wix Template to create my Portfolio Website

## Saturday July 1st, 2017
* Learnt some html tags: figure, fig caption, mark, abbr
* How to use the grid system when inserting multiple images on bootstrap.


## Sunday July 2nd, 2017
* Javascript commands: alert, console.log, prompt, conditional statement(if, else if, else)
* Also learnt how to use while loop, infinite loop, for loop, functions: arguments, return keyword.

## Monday July 3rd, 2017
* Used html to create form using javascript to get the values of the form with input type :name and birthday
* How to use e.preventDefault method to stop the default form action
* How to attach .addEventlistener to a specific function
* learnt how to link jquery google cdn.
* Below is the html-javascript form data:

*  <!DOCTYPE html>
+ <html>
<head>
  <meta charset="utf-8">
  <title>SyncFiddle</title>
  <style>
    body {
      font-family: "Helvetica Neue", Helvetica, sans-serif;
    }
  </style>
  
 <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
  
</head>
<body>
  
  <h1>Hello World</h1>

	<p>Today's Date is:</p>
	<p id='date' ></p>

  <p id="birthday"></p>
  

	<h3>Data List</h3>
  <hr />
	<ul id='dataList'>
  
	</ul>
  
  <h4>Your Birthday here</h4>
  <form id="bdayValidator">
    <label for="name">Name:</label>
    <input type="text" name="Name" id="name" placeholder="Name" required><br/>
<label for="bday">Birthday:</label>
    <input id="bday" type="date" required><br>
    
    <input type="submit" value="Show Birthday">
  </form>
  
  <script>
    
  function dateFunction(val) {
    return new Date();
  }
    
  function showBirthday(e) {
    e.preventDefault();
    var name = document.getElementById('name').value;
    var bday = document.getElementById('bday').value;
    console.log(bday, typeof (bday));
    document.getElementById('birthday').innerHTML = "Hello " + name + ", your birthday is: " + bday;
  }
    document.getElementById('bdayValidator').addEventListener('submit', showBirthday);
    
document.getElementById('date').innerHTML = dateFunction();

	// create show birthday button
	// attach a click event handler to the button
  // write the function
  // Prompt user for input
  // create a form
  // Add a name and date input
  // Add a submit button
  // Get data from name input
  // Get data from birthday input
  // Output data to html
  </script>
</body>
</html> 