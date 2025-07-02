<ul><li><a href="{{ site.url }}/tools">Back</a></li></ul>

<div style="width:100%; display:block;">

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

<div>
	<label for="safety">Safety factor:</label>
	<input type="number" id="safety" min="1" step="0.1" value="4.0" required>
</div>

<button onClick="calculate()">Calculate</button>
<div id="result"></div>

</div>

<script>
function calculateAquarium(length, width, height, safety){
	
	//input validation
	if(length <= 0 || width <=0 || height <=0){
		throw new Error("Dimensions must be positive numbers.");
	}
	
	//Convert dimensions from cm to m
	const heightM = height / 100;
	const lengthM = length / 100;
	const widthM = width / 100;
	
	
	//Calculate water pressure in pascals : p * g * h
	// p = watr density (1000 kg/m3), g = gravity(9.81 m/s2)
	const pressure = 1000 * 9.81 * heightM;
	
	//Maximum stress on glass
	
	const allowableStress = 19e6;
	const stress = (0.5 * pressure * lengthM * heightM) / (allowableStress / safety);
	
	
	const thicknessM = Math.sqrt(stress);
	const thicknessMM = thicknessM * 1000;
	
	//Calculate volume
	const volumeCm3 = length * width * height;
	const volumeLiters = volumeCm3 / 1000;
	
	//Standard glass thickness(mm)
	const standardThicknesses = [3, 4, 5, 6, 8, 10, 12, 15, 19, 25];
	
	//find the next standard thickness
	
	let recommendedThickness = standardThicknesses.find(t => t >= thicknessMM) || 25;
	
	
	return {
		volume: volumeLiters.toFixed(2),
		thickness: thicknessMM
		rthickness: recommendedThickness
	};
}

function calculate(){
	try {
		const length = parseFloat(document.getElementById('length').value);
		const width = parseFloat(document.getElementById('width').value);
		const height = parseFloat(document.getElementById('height').value);
		const safety = parseFloat(document.getElementById('safety').value);
		
		const result = calculateAquarium(length, width, height, safety);
		
		document.getElementById('result').innerHTML=`Water Volume: ${result.volume} liters<br>Recommended Glass Thickness: ${result.thickness} mm<br>Recommended Glass Thickness: ${result.rthickness} mm`;
		
	} catch(error){
		document.getElementById('result').innerHTML = `Error: ${error.message}`;
	}
}

</script>


