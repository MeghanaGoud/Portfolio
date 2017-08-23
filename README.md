# Portfolio
Build a great looking portfolio where we can show off images, descriptions and links to all of your projects, skills.
## Getting started
These instructions will help you to run the project on your local computer. See deployment for notes on how to deploy the project on a live system
### Prerequisites
Install sublime text latest version or visual studio or notepad++ for editing and writing our HTML file
### Instructions
Start the html file with DOCTYPE HTML and html tags as given below
```
<!DOCTYPE html>
```
For every opening tag there should be closing tag. And html file starts with the html tag `<html>….</html>` wat ever our html content it should be under these two html tags. `<head>….</head>` this tag includes the title and other references in `<link>` if we want to embedd the font family or any other url links we will embedd them in the head tag, as we are writing our html file in English it is advised to keep `lang=”en”` in the html tag.
```
<html lang=”en”> 
```
Now the entire head tag will be
```
<head>
	<meta charset="utf-8">
	<!--compatible in all devices-->
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>portfolio</title>
	<!--fonts references-->
	<link href=https://fonts.googleapis.com/css?family=Roboto:300,400,500 rel="stylesheet">
	<link href="https://fonts.googleapis.com/css?family=Oxygen" rel="stylesheet">
	<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
	<!--fonts ends here-->
        <link rel="stylesheet" href="css/style.css">	<!--css style sheet-->
</head>
```
That meta tag basically specifies what character set is your website written with. ...`UTF-8` (U from Universal Character Set + Transformation Format—8-bit) is a character encoding capable of encoding all possible characters (called code points) in Unicode. The encoding is variable-length and uses 8-bit code units.
One can add their script in the head or at the end of the body in script tag
```
<script>….</script>
```
If you want to add your style sheet in the html file itself then use the style tag, this type of styling is called internal styling
```
<style>….</style>
```
If we want to style only particular element we can write style in that particular tag and it is referred as inline styling
```
<p style=”font-size:20px;”>…</p>
```
Body section, class `container` is used to add padding or margin to the left and right. The content of our website will be in the body section
```
<body>..</body>
```
Logo and title are placed in header tag, control the positions of the logo and title using `float` as mentioned in the css file.
```
<header>..</header>
```
To add an additional description I have used a div and I adjusted the position by using absolute and margin.
```
Position:absolute;
Margin-left:auto;
Margin-right:auto;
```
After the description, projects block starts here, first define the width for each block and within that block adjust the width of the images to be `100%` in order to be responsive. And in order to display this blocks side by side use the property `flex`.
```
.projects img{
	width: 100%;	/*width is 100%*/
        }
.projects {
	Display: flex;	/*side by side*/
        }
```
Style the content in the blocks according to our interest in css file. Use the anchor tag to link to your repositories, and place all your content in the article tag and place this everything in a figure tag and use section tag if needed if you are using section tag you have to define an id or class to it. Follow HTML structural elements documentation to know more. Adjust the width and margin in responsive using media queries.
```
@media screen and (min-width: 320px) and (max-width: 768px) {
/*styling properties*/
} 
```
The above one is for the devices whose width is between 320 and 768px, similarly do that for different dimensions.
For skills and experience use different div tags represent your skills in your style similarly to your experience as well add your respective contact details in another division here I have used fa icons you can refer to that in W3schools font awesome icons.
### Run
save your html file with the .html extension and css with .css extension, maintain all your files in file structure i.e, css files in css folder similar to images and js files place all these folder in your project folder. Open your html file in different browsers and check your work





