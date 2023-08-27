# Friend
<img width="960" alt="image" src="https://github.com/FabAlcindor/WebDev_Friend/assets/142107701/814df274-b29b-4701-9551-907d4c15cdca">

<h1>Web Development Project</h1>
In this tutorial We will breakdown and use three different coding language to develop a simple game for kids to play. <br />

<h2>Environments and Technologies Used</h2>

- Visual Studio Code
  

<h2>Coding Language</h2>

- Javascript
- HTML5
- CSS
<h2>High-Level Steps</h2>

- Step 1: Use HTML to set up the "face" of website.
- Step 2: Use Javascript to give the the website functionality  
- Step 3: Use CSS to make the "face" more visually appealing
- Step 4: Make sure that the HTML file properly sources or references the javascript and css files. 

<h2>HTML</h2>

<p>
<img width="493" alt="image" src="https://github.com/FabAlcindor/WebDev_Friend/assets/142107701/a668f2f2-b3d9-4bdb-80f4-72c6c9d720fa">
</p>
<p>
First begin by opening a HTML file an typing out the boiler plate. Notice that the link element has a href, his is what references the CSS file which will be used to give the page color and style. For right now it can be ignored as it will be much easier to style everything once we have the face and function already set up.
</p>
<br />

<p>
<img width="398" alt="image" src="https://github.com/FabAlcindor/WebDev_Friend/assets/142107701/1871f83e-9329-4c33-ba20-8b3142158381">
</p>
<p>
Within the body section of html set up three div elemnets. Each one of these divs will hold a different parts of the project. Above the first div, set an empty h2 element and give it an ID. This will be very important for helping display questions. Inside the first div elements nest two more div elements. The first one will hold three buttons, and should be given a unique ID. For the purpose of this tutorial it is known as "pocket". The second one will hold only one button and will have the ID of "rest". Be sure to give the the parent div a unique id as well, mines will be known as "fold". The two other divs that aren't nested within "fold" should also be given unqiue ID's, and for the purpose of this tutorial will be referenced by them. Within "fold2" nest three buttons. Within "fold3" nest two p elements, both of which should be given an ID. Notice that the script element has a "src" , this is how html will be able to utilize the javascript file we will create later on.  The last few things for the html section is to add some classes, ID's, and text to certain elements. Starting with classes, ensure that "fold" and "fold2" have the class "choice". Also make sure that "fold" has the class "bye". These will make styling a lot easier since the class names can apply to multiple elements. All buttons should be given the "button" class name as well. The buttons should be given ID's as well. An important note is that at most only 4 buttons will be visible in the final product, so the ID's can differ to make it easier to read, but for us it will simply be "click" followed by a number. Next add the "onclick" tag to all the buttons. There is one button that is nested in a nested div known as "rest" the button should be given the ID of "reset" as that is what it will function as. The last thing to do is add text to the p elements. They will function as visual counters and should be named for what they count. In this case the first represents the "Friendship score" while the second represents "Days passed". "reset" should also be given text matching its ID.
<br />

<h2>Javascript</h2>
<p>
This section will be divided up into smaller subsections to give each one the attention it deserves. The code will not properly function until everything is set up so it will be a bit of a process.
</p>

<h3>Variables</h3>

<img width="309" alt="image" src="https://github.com/FabAlcindor/WebDev_Friend/assets/142107701/c16d1c6f-4acd-4791-8eb9-6f2853ea694a">

<p>
The first of the subsection focuses on the varibales needed to make things work in a certain way. Given that Varibles can represent different outcomes it's ideal to specficy whenever possible what outcome you want. Notice that the first three variabels are all asigned the value of "0". This tells javascript that the varible is expected to be a number and that it's current value is 0. Variables can also represent strings which is the case for all the other variables. "X" and "Y" will change the current text of the two p elements from the previous section, to match that of the current value of the "friend" and "day" variabels. The last set of varibles will be used to alter the class list of the divs, allowing us to add or remove certain classes from the divs. 
</p>
<br />

