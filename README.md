# Static Website: New York City Blog

## Overview
After researching New York City, you decide to create a blog for your viewers who want to know more about the city. It’s time to create a blog to show off how amazing the Big Apple is. You got this!

Don’t forget to save your code after each step. By pressing save to run your code you will see the changes you’ve made in the browser.

Note: While you are developing the webpage, you will notice that the elements are automatically assigned colors, borders, and positioned properly. This is because of the CSS file. Don’t worry about CSS right now, it’s only there so that the webpage looks nice.

![image]()

## HTML
```
<!DOCTYPE html>
<html>
   <head>
      <link rel="stylesheet" href="style.css">
   </head>
   <body>   
     <nav>
       <ul>
         <li><a href="">Blog</a></li>
         <li><a href="">Media</a></li>
         <li><a href="">About</a></li>
       </ul>
     </nav>
     <header>
       <h1>New York City</h1>
     </header>
     <main>
       <section id="blog">
         <article>
           <p>New York City is made up of five boroughs which include Queens, Manhattan, Brooklyn, the Bronx, and Staten Island. The city is the home of approximately 8 million people. In 1876, France gifted the City of New York what is known as the Statue of Liberty, which is currently located on Ellis Island commonly visited by tourists. However, it took 10 years to assemble and therefore wasn’t unveiled until 1886. Another tourist destination is Times Square. Times Square is commonly known for the big buildings, Broadway shows, and bright neon signs. This famous location was named after The New York Times after the Times moved to that location. Prior to that, it was named Longacre Square. New York City is also known for its bridges that connect the boroughs and allow ease of transportation.</p>
           <figure>
             <img src="https://content.codecademy.com/courses/Semantic%20HTML/statue-of-liberty.jpeg">
             <figcaption>This is the Statue of Liberty, a popular tourist attraction located on Ellis Island.</figcaption>
           </figure>
           <aside>
             <p>New York City is very popular for the variety of great food it has. Some of the top food items in NYC include:</p>
             <ol>
               <li>Pizza</li>
               <li>Bagels</li>
               <li>Burgers and Sandwiches</li>
               <li>Ramen</li>
               <li>Tacos</li>
               <li>Pasta</li>
               <li>Desserts</li>
              </ol>
              <section id="media">
                <article>
                  <h2>The Scenery in NYC</h2>
                  <p>While the view in the city is beautiful, the sounds are not as lovely. Below you'll see an example of the view and the sounds you'll deal with in NYC on a daily basis.</p>
                </article>
                <video src="https://content.codecademy.com/courses/Semantic%20HTML/nyc-skyline-timelapse.mp4" controls>Video not found</video>
                <embed src="https://content.codecademy.com/courses/Semantic%20HTML/nyc-skyline.jpeg">
                <audio src="https://content.codecademy.com/courses/Semantic%20HTML/nyc-sounds.mov" controls>Audio not found</audio>
              </section>
           </aside>
         </article>
       </section>
     </main>
     <footer>
       <p>Posted by</p>
       <p>Contact information: Blogger@NYC.com</p>
       </footer>
     
     
     
   </body>
</html>
```

## CSS
```
body {
	background: #e6e6e6;
}

nav ul {
	list-style-type: none;
	margin: 0;
	padding: 0;
	overflow: hidden;
	background-color: #010e80;
	display: table;
	width: 100%;
}

nav li {
	display: table-cell
}

li a {
	display: block;
	color: white;
	text-align: center;
	padding: 30px 30px;
	text-decoration: none;
}

li a:hover {
	background-color: #111;
}

h2 a {
	padding: 33px 25px;
	color: white;
	text-decoration: none;
}

h2 a:hover {
	background-color: #111;
}

figcaption{
  text-align:left;
}

header {
	margin-left: 14px;
}

article {
	text-align: left;
	margin: 15px;
	max-width: 80%;
	font-size: 18px;
	line-height: 32px;
}

img {
	width: 400px;
	height: 300px;
  position:relative;
  right:28px;
}

aside {
	left: 10px;
	border: 1px solid black;
	padding: 15px;
	max-width: 80%;
	position: relative;
	border-color: #010e80;
	border-width: 5px;
	font-size: 18px;
}

footer {
	position: relative;
	width: 100%;
	bottom: -100px;
	background-color: #010e80;
}

footer p {
	color: white;
	text-decoration: none;
	padding: 10px;
	text-align: center;
	width: 100%;
	box-sizing: border-box;
}

footer a {
	color: white;
	text-decoration: none;
	text-align: center;
	width: 100%;
}

video {
	display: block;
	width: 420px;
	height: 250px;
  padding:15px;
}

audio {
	padding: 15px;
	width: 98%;
  box-sizing: border-box;
}

embed {
	width: 400px;
	height: 458px;
  padding:15px;
}
```