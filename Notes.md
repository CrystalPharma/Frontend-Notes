# Bootcamp Notes
## Fundamental Javascript
## Javascript 
JavaScript is a programming language that allows programmers to implement complex features on web pages — every time a web page does more than just sit there and display static information for you to look at — displaying timely content updates, interactive maps, animated 2D/3D graphics, scrolling video jukeboxes, etc. 

## JavaScript engine
-	Converts human readable codes into machine code without producing intermediate codes
-	Many of the JavaScript engine to date are JIT compilers (just in time compilers) that produce in time translation and optimisation 

## Console windows/ interfaces
- Allow to input commands and view outputs
- Input commands to console, taken live to JavaScript JIT engine compiled, processed and presented viewing the outputs of the commands delivered into human readable format texts 
- useful in debugging and reviewing any errors in inputting codes and highlight in the Console window
- Consoles are opened in common developer tools

## Console.log
Console.log is a function that prints message that exits in the Javascript engine
- it is particularly impprtant to test whether the code is functioning as intended

## Variables 
(Noun) in Javascript in the following forms:
- numbers  (1)
- strings ("string")
- Booleans (true, false)
etc.

## Arithmetic operators


## Array (arr)


## Object

## Method

## API
Application Programming Interface
- provide a way for creating user code that utilises pre-built code to conduct various tasks.
## API Key & importance of its access
API key is used by multiple web APIs, that provide access control (for identification).
API key usually is related to the identification of API user also different rights (i.e.quota and authorisation area) that are open for access to the key
- applies to HTTPS for example

## Query String
General thumb of rule in URL:
protocal (HTTP/ HTTPS), location of file/ program (in form of host-name/ file-name) and query string

- length limitation
Try to limit the length of query strength (depends on the server ability to handle MAX 2000)
> The HTTP protocol does not place any a priori limit on the length of
   a URI. Servers MUST be able to handle the URI of any resource they
   serve, and SHOULD be able to handle URIs of unbounded length if they
   provide GET-based forms that could generate such URIs. A server
   SHOULD return <b>414 (Request-URI Too Long) status</b> if a URI is longer
   than the server can handle (see section 10.4.15).

## Use of API Key (with examples)

<code>
//use of concatanation to clean code <br>
var apiKey = 'trilogy'; <br>
var queryURL = "https://www.omdbapi.com/?t=dune&y=&plot=short&apikey=" + apiKey;
</code>

## API endpoint
APi endpoint is
Specific digital location where that allows communication and connections between sofeware programs (via exchange of code)
- requests for information are sent by one program to retrieve pre-existing digital resource 

>Sending request for information from web application/ server ➡ Receive response 

<b>Example : Instagram</b>

- business and creators endpoint that measure media and profile interactions
- moderation endpoint that regulate comments and replies
- discovery of hashtagged media 
etc.

## JSON
JavaScript Object Notation
it is a common format that data will be presented via an API.

## AJAX
Asynchronous JavaScript And XML. It is nota programming language but rather a technology <br>
It allows us to update web pages by exchanging data with a web server, without reloading the page

### .then() function

## Break into pieces
User input -> response -> output




