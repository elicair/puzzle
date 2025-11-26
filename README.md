# puzzle
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Three Sections Grid</title>
<style>
body {
margin: 0;
font-family: Arial, sans-serif;
}
.grid-container {
display: grid;
grid-template-columns: 1fr 1fr 1fr; /* three equal columns */
gap: 10px;
}
.section {
padding: 20px;
background-color: #f0f0f0;
border: 1px solid #ccc;
}
</style>
</head>
<body>
<div class="puzzle-container">
<img src="images/puzzle1.png" class="puzzle-piece" data-fit="true" />
<img src="images/puzzle2.png" class="puzzle-piece" data-fit="true" />
<img src="images/puzzle3.png" class="puzzle-piece" data-fit="false" /> <!-- does not fit -->
<!-- more pieces -->
</div>

<style>
.puzzle-container {
display: flex;
flex-wrap: wrap;
gap: 10px;
}
.puzzle-piece {
width: 100px;
height: auto;
}
</style>

<script>
// Hide pieces that do not fit
document.querySelectorAll('.puzzle-piece').forEach(piece => {
if (piece.dataset.fit === 'false') {
piece.style.display = 'none';
}
});
</script> 
<div class="grid-container">
<div class="section">Section 1: Welcome to the page</div>
<div class="section">Section 2: About us</div>
<div class="section">Section 3: Contact info</div>
</div>
</body>
</html>   
