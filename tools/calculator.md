<ul><li><a href="{{ site.url }}/tools">Back</a></li></ul>

<h1>Aquarium calculator</h1>

<p>Enter dimensions in centimeters:</p>

<div>
	<label for="length">Length:</label>
	<input type="number" id="length" min="1" step="1" required>
</div>

<div>
	<label for="width">Width:</label>
	<input type="number" id="width" min="1" step="1" required>
</div>

<div>
	<label for="height">Height:</label>
	<input type="number" id="height" min="1" step="1" required>
</div>

<button onClick="calculate()">Calculate</button>
<div id="result"></div>
<script>
function calculateAquarium(legnth, width, height){
	
	//input validation
	if(length <= 0 || width <=0 || height <=0){
		throw new Error("Dimensions must be positive numbers.");
	}
	
	//Calculate volume (90% of height for water level)
	
	const waterHeight = height * 0.9;
	const volumeCm3 = lenght * width * waterHeight;
	const volumeLiters = volumeCm3 /1000;
	
	
	//Calculate glass thikness
	let thickness = 0.015 * height * Math.sqrt(length * width) + 1;
	if(height > 60 || volumeLiters > 500) {
		thickness *= 1.5;
	}
	
	//Standard glass thickness(mm)
	const standardThicknesses = [4, 5, 6, 8, 10, 12, 15, 19, 25];
	
	//find the next standard thickness
	
	let recommendedThickness = standardThicknesses.find(t => t => thickness) || 25;
	
	
	return {
		volume: volumeLiters.toFixed(2),
		thickness: recommendedThickness
	};
}

function calculate(){
	try {
		const length = parseFloat(document.getElementById('length').value);
		const width = parseFloat(document.getElementById('width').value);
		const height = parseFloat(document.getElementById('height').value);
		
		const result = calculateAquarium(length, width, height);
		
		document.getElementById('result').innerHTML='Water Volume: ${result.volume} liters<br>Recommended Glass Thickness: ${result.thickness} mm';
		
	} catch(error){
		document.getElementById('result').innerHTML = error.message;
	}
}

</script>


