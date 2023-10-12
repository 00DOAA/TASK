# TASK
<!DOCTYPE html>
<html>
<head>
	<title>Calculator</title>
</head>
<body>
	<h1>Calculator</h1>
	<form>
		<input type="text" id="num1" placeholder="Enter first number">
		<input type="text" id="num2" placeholder="Enter second number">
		<br><br>
		<button type="button" onclick="add()">Add</button>
		<button type="button" onclick="subtract()">Subtract</button>
		<button type="button" onclick="multiply()">Multiply</button>
		<button type="button" onclick="divide()">Divide</button>
		<br><br>
		<label>Result:</label>
		<input type="text" id="result" readonly>
	</form>

	<script>
		function add() {
			var num1 = parseFloat(document.getElementById("num1").value);
			var num2 = parseFloat(document.getElementById("num2").value);
			var result = num1 + num2;
			document.getElementById("result").value = result;
		}

		function subtract() {
			var num1 = parseFloat(document.getElementById("num1").value);
			var num2 = parseFloat(document.getElementById("num2").value);
			var result = num1 - num2;
			document.getElementById("result").value = result;
		}

		function multiply() {
			var num1 = parseFloat(document.getElementById("num1").value);
			var num2 = parseFloat(document.getElementById("num2").value);
			var result = num1 * num2;
			document.getElementById("result").value = result;
		}

		function divide() {
			var num1 = parseFloat(document.getElementById("num1").value);
			var num2 = parseFloat(document.getElementById("num2").value);
			var result = num1 / num2;
			document.getElementById("result").value = result;
		}
	</script>
</body>
</html>
