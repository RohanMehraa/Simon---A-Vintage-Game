# Simon---A-Vintage-Game

Simon is a Vintage game very popular in 198X.
Simon is an electronic game of memory skill invented by Ralph H. Baer and Howard J. Morrison, working for toy design firm Marvin Glass and Associates, with software programming by Lenny Cope. The device creates a series of tones and lights and requires a user to repeat the sequence. Wikipedia
Introduced: 1978
Publisher: Milton Bradley Company (now Hasbro)
Availability: 1978–present
Inventor(s): Ralph H. Baer and Howard J. Morrison


To implement it using javascript, Let us understand it's working:

Firstly, the game shows the first colour in the sequence (suppose blue). The user clicks on the blue button.

Next, the game shows the next colour (red), the user has to remember the sequence is blue, red and so on and so forth.

If the user messes up the sequence, then the game ends. 



NOTES:
JAVASCRIPT/JQUERY:

document.querySelector("h1");
document.querySelectorAll("h1");

=> $("h1");
// the $ in jQuery is equivalent to document.querySelector, document.querySelectorAll of javascript.

=> $("h1").css("color", "red");  //When two parameters are given, it "sets" the property of element to red.
=> $("h1").css("color");  //when passed single parameter it "returns" the color property already applied on the element h1.

=> $("h1").addClass("big-heading");
=> $("h1").addClass("big-heading white-color");

=> $("h1").removeClass("white-color");
=> $("h1").removeClass("big-heading white-color");

=> $("h1").hasClass("white-color");
//returns a boolean value true or false based on whether that particular class in applied on this element or not.

document.querySelector("h1").textContent;  //javascript code
=> $("h1").text("Hello"); //updates text inside the h1 element.


document.querySelector("h1").innerHTML;  //javascript code
=> $("h1").html("<em> BYE </em>");

$("a").attr("href");  //gets the href attribute of 'a' anchor tag.
$("a").attr("href", "google.com");  //sets the attribute value to "google.com" of ALL the 'a' anchor tag.

=> $("h1").hasClass("white-color");
//returns a boolean value true or false based on whether that particular class in applied on this element or not.

ALTERNATIVELY,
("h1").attr("class");  //this will return the value of all the classes applied to all the "h1" elements.




//javascript code
for (var i = 0; i < totalDrumBtn; i++) {
  document.querySelectorAll("button")[i].addEventListener("click", function () {
    
      document.querySelector("h1").style.color("purple");

  });
}

=>jQuery code:
$("button").click(function (){
    ("h1").css("color", "purple");
});


//keypress javascript code:
document.addEventListener("keypress", function (event) {
  makeSound(event.key);
  buttonAnimation(event.key);

=> $("document").keypress(function (event) {
    console.log(event.key);
});

ALTERNATIVELY,

=> $("h1").on("<event_type>", <callbackFunction> () {
    $("h1").css("color", purple); 
});


ADD ELEMENTS USING JQUERY:

$("h1").before("<button> NEW </button>");  //adds button element before the h1 tag.

$("h1").after("<button> NEW </button>");    //adds the button element after the h1 tag.

$("h1").prepend("<button> NEW </button>");  //adds the button element inside the h1 tag and before it's inner value. for eg: <h1> <button> NEW </button> HELLO </h1>

$("h1").append("<button> NEW </button>");  //adds the button element inside the h1 tag and after it's inner value. for eg: <h1> HELLO <button> NEW </button> </h1>



$("button").remove(); will remove all the button elements from the html doc. 
