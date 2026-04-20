"# Vector" 
<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Vector Calculator UI</title>

<style>
    body {
        font-family: 'Segoe UI', sans-serif;
        background: linear-gradient(135deg, #667eea, #764ba2);
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        margin: 0;
        color: white;
    }

    .container {
        background: rgba(255,255,255,0.1);
        backdrop-filter: blur(12px);
        padding: 30px;
        border-radius: 20px;
        width: 360px;
        box-shadow: 0 10px 30px rgba(0,0,0,0.3);
    }

    h1 {
        text-align: center;
        margin-bottom: 20px;
    }

    label {
        font-size: 14px;
        margin-top: 10px;
        display: block;
    }

    input, select {
        width: 100%;
        padding: 10px;
        margin-top: 5px;
        border-radius: 10px;
        border: none;
        outline: none;
        background: rgba(255,255,255,0.2);
        color: white;
    }

    input::placeholder {
        color: rgba(255,255,255,0.7);
    }

    .vector-group {
        margin-top: 15px;
    }

    .result-box {
        margin-top: 20px;
        padding: 15px;
        border-radius: 10px;
        background: rgba(0,0,0,0.2);
        text-align: center;
        font-size: 18px;
    }

    .button {
        margin-top: 15px;
        padding: 12px;
        border-radius: 12px;
        background: #00c6ff;
        text-align: center;
        font-weight: bold;
        cursor: pointer;
    }
</style>

</head>
<body>

<div class="container">
    <h1> คำนวณ Vector</h1>

    <label>Dimension</label>
    <select>
        <option>2D</option>
        <option>3D</option>
    </select>

    <div class="vector-group">
        <label>Vector A</label>
        <input placeholder="A[1]">
        <input placeholder="A[2]">
        <input placeholder="A[3]">
    </div>

    <div class="vector-group">
        <label>Vector B</label>
        <input placeholder="B[1]">
        <input placeholder="B[2]">
        <input placeholder="B[3]">
    </div>

    <label>Operation</label>
    <select>
        <option>A + B</option>
        <option>A - B</option>
        <option>Dot Product</option>
        <option>|A|</option>
        <option>|B|</option>
    </select>

    <div class="button">
        Calculate
    </div>

    <div class="result-box">
        Result will appear here
    </div>
</div>

</body>
</html>
