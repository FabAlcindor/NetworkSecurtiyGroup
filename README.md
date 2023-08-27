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
<img width="413" alt="image" src="https://github.com/FabAlcindor/WebDev_Friend/assets/142107701/0cd35ed5-6825-4c2c-b425-7d2a3810ec47">
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
The first of the subsection focuses on the varibales needed to make things work in a certain way. Given that Varibles can represent different outcomes it's ideal to specficy whenever possible what outcome you want. Notice that the first three variabels are all asigned the value of "0". This tells javascript that the varible is expected to be a number and that it's current value is 0. Variables can also represent strings which is the case for all the other variables. "X" and "Y" will change the current text of the two p elements from the previous section, to match that of the current value of the "friend" and "day" variabels. The last set of varibles will be used to alter the class list of the divs, allowing us to add or remove certain classes from the divs. The way we are able to specfiy which element to tinker with is through the use of IDs which are unique to each element assigned one. This is done through the "getElementById()", then specficy the ID.
</p>
<br />
<h3>Array</h3>
<img width="811" alt="image" src="https://github.com/FabAlcindor/WebDev_Friend/assets/142107701/543cc3fe-2ca9-4c48-93c3-a6e616885afd">

<P>
This section focuses on one of the most important pieces of the code, an array. The array is what will hold all the information for choices, scenarios and questions. The array has two levels to it, the first layer is what we will use to determine what story is selected. The second layer is where we will pull the relavent information. The array will contain a whole host of objects that we will use to applay text to the buttons and p elements. Ideally use comments to help seperate and keep track of both the number of entries as well as what story it is.  Javascript  uses indexing to count, which means it starts at zero rather than one. This is important as it allows us to create a section specfic to the "day" and "story" values being set to 0, This is mentioned as the "Welcome Message". There are a total of 7 objects type we will have to worry about for this tutorial. The first is "question_text" which will be the text that is shown on the h2 element in html. There is three "choice" and three "_choice" that will help to display the responses on the buttons. The three "choice" only have a single entry as they will be used to help navigate to which story the user wants to select.The other "_choice" represent a positve, negative or neutral choice that the player can make and have alot of entries. The reason for the seperate object types is due to how the objects are assigned to the buttons. There are effectivly two sets of buttons, however only one set can be active at a time. Since the buttons will be tied to different functions seperating them but making on inactive, helps to prevent unwanted outcomes, such as accidentally changing the story mid-way.  For the specfic text in each of the objects, it is purely up to the developer.
</P>

<h3>Functions</h3>
<img width="256" alt="image" src="https://github.com/FabAlcindor/WebDev_Friend/assets/142107701/f7c393ca-9594-4a12-9c5c-9d76a925e73d">
<p>
  This subsection will focus on the four functions that are necessary to allow for functionality of the program. Each function will serve a very necsaary part of the code and to a degree rely on one another. 
  
  The first of the functions is the one named "pals". The purpose of this function is to adjust the counters in a specfic way. This function takes in an argument known as "num", which is then added to the current value of friend to give it a new value. The variable "day" is increased by one through the "++" method. Lastly "x" and "Y" are updated to reflect the new values of friendship score and day respectively.

  The second of the functions is "book". This function also accepts an argument knwon as "chap", which will change the value of "story" when the function is called. The function will also remove the class "bye" from "fold".
</p>
<br />
<img width="740" alt="image" src="https://github.com/FabAlcindor/WebDev_Friend/assets/142107701/1b228e2c-836e-4cfd-942a-fe3f6fb670e1">
 <p>The third function is repsobile for replacing the text on buttons and the h2 element whenever a question is answered. It also is responsible for printing the ending quotes based on the friendship score. 
   
   The first step is to ensure that the right buttons appear, which is handled whenever the value of story is higher than 0. The sence function will add the "bye" class to "fold2" which will make sense when the CSS section comes up.
   
   The second step is to create a new varible, mines is known as "dc". Set the new varible to be equal to "lore" but indexed at certain points equivivalent to the current value of "story" and "day". With the way that the array functions, it's imperative that it is done in that order to prevent unwanted outcomes.
   
   The third step is where a the magic happens. Using an "if else" statement, the function will check to see if the current value of "day" is below the total number of items in the sub-array found in "lore". This does not check the entire amount of items in lore, but only the nested one found at an index value equal to the current value of "story". If the value of day does not exceed the total amount of items of "lore[story]", then the function will use "dc" to pull new information to replace old information. Using "lore[story][day]" it will assign each button a specfic string using "getElementById". This will work for the welcome message as well even though they are rarely used. By using "innerHTML", we are able to changce the text of what the buttons say. We can then use "dc.___" to assign an object to the element. For example lets say that the current value of "story" is one, while the current value of "day" is zeor. When javascript reaches the scene function it will look at the line "document.getElementById("question").innerHTML = dc.question_text" and begin by identifying the value of dc. This would be seen as "lore[1][0]". It would then look at the property "question_text"  at that specfic point in the array to produce a the text "It's your first day at school, what will you do when you meet your classmates?". Next, we need to handle the "else" aspect of the statement. This is what will happen when the value of "day" is equal to or exceeds the total number of objects in "lore[story]". This is where we then add a second "if else". This "if else" statement will check the value of "friend" to produce a specfic end response.  Within the "lore" array it contains three sub-arrays which in turn contain seven objects each. Using that set the high and low of max point values to be the positive and negative versions. I reccomend adding one for zero as well as its represents a neutral outcome. Outside of that feel free to add as many as you may feel is necessary. I added two more which will check to see if the value of "friend" is between 0 and 7 or between -7 and 0. Now once the value of "day" is at least the same as the number objects in the array, we will want to apply the "bye" class to "pocket" so that we can hide the some of the buttons. We can also change the text of "reset" so that it ask "Play Again?". 
</p>

<img width="361" alt="image" src="https://github.com/FabAlcindor/WebDev_Friend/assets/142107701/7042a08f-b40a-47a1-839f-7c89e9dc7440">

<p>
  The last function is the "reset()" fucntion. This handles the fucntionality button of the same name by adjusting the values of key variables. First start out by directly changing the value of "friend", "story", and "day" to zero. Using "beta" and "delta" and the line the "classlist.remove" to remove the "bye" class from "fold2" and "pocket". Second using "alpha" and "classlist.add" to add "bye" to "fold". Next make sure to update the displayed values of "freindship score" and "day". The last thing needed is to change the "reset" button to say "Reset". After that make sure to call "scene()"to make sure all things are properly updated. This should be done both at the end of the code, as well as the end of "reset()" just to make sure the scene does update.
</p>


<h3>Linking it all</h3>
<img width="440" alt="image" src="https://github.com/FabAlcindor/WebDev_Friend/assets/142107701/0e3a0866-5cc4-4177-a7cd-e3d6f1923f55">

<p>
  The last thing we will need to finally establish fucntionality, is to link javascript to html. First start with the script element. add "src=" and the name of the javascript file. Next is to add calls to the functions. Going back to the buttons in the html file, it's time to add the calls. First, for all buttons except "reset" add the "scene()" to each onclick. In "fold" and the "pals()" call. Since this function accepts an argument you can set a value to each button by putting "pals(0)". The values should be "1","0", and "-1". This should be applied to the respective choice. a positive choice should increase friend not decrease. In "fold2" add "book()" to the onclick on each of the buttons. This function also accepts arguments but this one should have values between "1" and "3" to represent each of the stories. If all has been done properly, the html file now has functionality and should be able to work pretty well, but not perfect.
</p>

<h2>CSS</h2>

<img width="417" alt="image" src="https://github.com/FabAlcindor/WebDev_Friend/assets/142107701/b97b0ce2-154e-4786-886b-3ea2b37d3c55">

<p> CSS is the easiest of the three and affects how everything looks, bringing color and style to the file. Only a few things are absolutely necessary to have, while most else is up to the preference of the developer. using the all selector "*" apply a "text-algin" and "align-items" and set both to center. Next add a class selector for the class "choice". Set "display" to "flex", "justify-content" to "center", and "flex-direction" to "row". Laslty is to add a class selector for "bye" which should have "display" set to "none". This is done so it could hide the buttons that aren't in use to prevent misclicks. After that head back to html file and in the link element set "href=" to the name of your css file. If done correctly then some of the buttons will disappear. After that feel free to give the buttons some colors or change the font of the text.
</p>
