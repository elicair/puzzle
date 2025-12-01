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
<img src="puzzle1_A.jpg class="puzzle-piece" data-fit="true" />
<img src="puzzle1_B.jpg" class="puzzle-piece" data-fit="true" />
<img src="puzzle1_C.jpg" class="puzzle-piece" data-fit="true" />
<img src="puzzle1_D.jpg" class="puzzle-piece" data-fit="true" />
<img src="puzzle1_E.jpg" class="puzzle-piece" data-fit="true" />
<img src="puzzle1_F.jpg" class="puzzle-piece" data-fit="true" />
<img src="puzzle1_G.jpg" class="puzzle-piece" data-fit="true" />
<img src="puzzle1_H.jpg" class="puzzle-piece" data-fit="true" />
<img src="puzzle1_I.jpg" class="puzzle-piece" data-fit="true" />
<img src="puzzle1_J.jpg" class="puzzle-piece" data-fit="true" />
<img src="puzzle1_K.jpg" class="puzzle-piece" data-fit="true" />
<img src="puzzle1_L.jpg" class="puzzle-piece" data-fit="true" />
<img src="puzzle1_M.jpg" class="puzzle-piece" data-fit="true" />
<img src="ipuzzle1_N.jpg" class="puzzle-piece" data-fit="true" />
<img src="puzzle1_O.jpg" class="puzzle-piece" data-fit="true" />
<img src="puzzle1_P.jpg" class="puzzle-piece" data-fit="true" />
<img src="puzzle1_Q.jpg" class="puzzle-piece" data-fit="false" /> <!-- does not fit -->
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
