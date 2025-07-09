# NetFlix_Clone
## Date:09.07.2025
## Objective:
To create a modern, responsive navigation bar using CSS Flexbox, mimicking real-world websites like Netflix. This helps reinforce alignment, spacing, and layout structuring using Flexbox properties.

## Tasks:

#### 1. Structure the HTML Layout:
Use a ```<nav>``` tag as the main container.

Add a brand logo/title on the left using a ```<div> or <h1>```.

Add navigation links like Home, Menu, About, Contact, and Login using a ```<ul> with <li> and <a>```.

#### 2. Apply Flexbox for Layout:
Use display: flex on the ```<nav>``` container.

Use justify-content: space-between to align the logo and menu.

Use align-items: center to vertically center both sections.

Style list items with horizontal spacing using gap or margin.

#### 3. Style Like a Real-World Navbar:
Add background color (e.g., dark or gradient like Netflix/Zomato).

Style text with bold fonts, hover effects, and link styling.

Remove default ul and li styles (list-style: none, text-decoration: none).

#### 4. Bonus Enhancements:
Add a hover underline or button effect on links.

Make it responsive using flex-wrap or media queries.

Fix the nav bar to top with position: sticky.
## HTML Code:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Netflix UI</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="container">
    <div class="header">
      <div class="date">
        <h2>NETFLIX</h2>
        <p>| Friday Feb 19</p>
      </div>
      <div class="menu">
        <p>Home</p>
        <p>Movies</p>
        <p>TV Shows</p>
        <p>My List</p>
      </div>
      <div class="icon">
        <img src="Rohith.jpg" width="30">
      </div>
    </div>

    <div class="centerbody">
      <div class="content">
        <p class="tags">DOCUMENTARY | TV SHOW | KNOWLEDGE</p>
        <h1>PEACE</h1>
        <p class="details">2022 | DIRECTOR : ABC CORP | SEASON 1 (1 Episodes)</p>
        <p class="desc">This documentary uncovers the major conflicts around the world.<br>Trying solve the Mysterious of Global powers and Military Capabilities.</p>
        <div class="buttons">
          <button class="stream">STREAM NOW</button>
          <button class="episodes">ALL EPISODES</button>
        </div>
      </div>
      <div class="rightside">
        <p class="trailer"><span>&#9658;</span> Watch Trailer</p>
        <div class="age">18+</div>
      </div>

      
    </div>
    <div class="popular-shows">
    <h3>POPULAR SHOWS THIS WEEK</h3>
    <div class="show-list">
      <div class="show"><img src="OIP (1).webp"><p>Squid game</p></div>
      <div class="show"><img src="OIP (2).webp"><p>Wednesday</p></div>
      <div class="show"><img src="OIP (3).webp"><p>Stranger Things</p></div>
      <div class="show"><img src="OIP (4).webp"><p>One piece</p></div>
    </div>
  </div>
  </div>
</body>
</html>
```
## CSS Code:
```
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Segoe UI', sans-serif;
}

body {
  background-color: red;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.container {
  background-color: black;
  height: 600px;
  width: 1200px;
  box-shadow: 4px 4px 10px rgba(0, 0, 0, 0.5);
  display: flex;
  flex-direction: column;
  gap: 20px;
  padding: 20px 40px;
  overflow: hidden;
  position: relative;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: white;
}

.date,
.menu,
.icon {
  display: flex;
  gap: 10px;
  align-items: center;
  color: white;
}

.menu p {
  cursor: pointer;
}

.centerbody {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  flex-grow: 1;
  margin-top: 20px;
}

.content {
  color: white;
  display: flex;
  flex-direction: column;
  gap: 15px;
  max-width: 600px;
}

.content .tags {
  font-size: 14px;
  color: gray;
}

.content h1 {
  font-size: 60px;
  letter-spacing: 2px;
}

.content .details {
  font-size: 14px;
  color: lightgray;
}

.content .desc {
  font-size: 13px;
  line-height: 1.4;
  color: gray;
}

.buttons {
  display: flex;
  gap: 15px;
}

.stream {
  background-color: red;
  color: white;
  border: none;
  padding: 10px 15px;
  font-weight: bold;
  cursor: pointer;
}

.episodes {
  background-color: transparent;
  color: white;
  border: 1px solid white;
  padding: 10px 15px;
  cursor: pointer;
}

.rightside {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  justify-content: space-between;
  height: 100%;
  padding-right: 20px;
}

.trailer {
  color: white;
  font-size: 14px;
  display: flex;
  align-items: center;
  gap: 5px;
  cursor: pointer;
}

.trailer span {
  font-size: 20px;
}

.age {
  background-color: red;
  color: white;
  padding: 5px 10px;
  font-size: 14px;
  border-radius: 3px;
  align-self: flex-end;
}

.popular-shows {
  color: white;
  margin-top: 20px;
  padding: 0 40px;
}

.popular-shows h3 {
  font-size: 16px;
  margin-bottom: 10px;
}

.show-list {
  display: flex;
  gap: 20px;
}

.show {
  display: flex;
  flex-direction: column;
  align-items: center;
  font-size: 12px;
  text-align: center;
}

.show img {
  width: 100px;
  height: 70px;
  object-fit: cover;
  border-radius: 5px;
}

.icon img{
  border-radius: 100%;
}
```
## Output:
![Screenshot 2025-07-09 231217](https://github.com/user-attachments/assets/1de88e21-1af6-4f07-b134-19ff2e7becc3)

## Live Webpage:

## Result:
A modern, responsive navigation bar using CSS Flexbox, mimicking real-world websites like Netflix. This helps reinforce alignment, spacing, and layout structuring using Flexbox properties is created successfully.
