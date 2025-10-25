<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>2D Realistic Music CD</title>
<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  body {
    height: 100vh;
    background: radial-gradient(circle at center, #222 0%, #000 100%);
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
    font-family: 'Poppins', sans-serif;
  }

  .cd {
    position: relative;
    width: 250px;
    height: 250px;
    border-radius: 50%;
    background: conic-gradient(
      #f5f5f5 0deg,
      #dcdcdc 30deg,
      #b3b3b3 60deg,
      #f0f0f0 120deg,
      #ccc 180deg,
      #e6e6e6 240deg,
      #f5f5f5 360deg
    );
    box-shadow: inset 0 0 20px rgba(255,255,255,0.3),
                inset 0 0 40px rgba(0,0,0,0.4),
                0 10px 25px rgba(0,0,0,0.6);
    animation: spin 20s linear infinite;
  }

  @keyframes spin {
    from { transform: rotate(0deg); }
    to { transform: rotate(360deg); }
  }

  /* Inner circle (label area) */
  .cd::before {
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    width: 80px;
    height: 80px;
    background: radial-gradient(circle, #f8f8f8 0%, #ccc 100%);
    border-radius: 50%;
    transform: translate(-50%, -50%);
    box-shadow: inset 0 2px 4px rgba(0,0,0,0.3);
  }

  /* Center hole */
  .cd::after {
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    width: 20px;
    height: 20px;
    background: #111;
    border-radius: 50%;
    transform: translate(-50%, -50%);
    box-shadow: inset 0 0 5px rgba(255,255,255,0.2);
  }

  /* Light reflection */
  .shine {
    position: absolute;
    top: 0;
    left: 0;
    width: 250px;
    height: 250px;
    border-radius: 50%;
    background: conic-gradient(
      from 180deg,
      rgba(255, 255, 255, 0.4) 0deg,
      transparent 60deg,
      rgba(255, 255, 255, 0.2) 120deg,
      transparent 180deg,
      rgba(255, 255, 255, 0.1) 240deg,
      transparent 300deg,
      rgba(255, 255, 255, 0.3) 360deg
    );
    mix-blend-mode: screen;
  }

  /* Rainbow reflection layer */
  .rainbow {
    position: absolute;
    top: 0;
    left: 0;
    width: 250px;
    height: 250px;
    border-radius: 50%;
    background: conic-gradient(
      red 0deg,
      orange 30deg,
      yellow 60deg,
      lime 90deg,
      cyan 120deg,
      blue 150deg,
      violet 180deg,
      red 360deg
    );
    opacity: 0.2;
    mix-blend-mode: screen;
    animation: shimmer 6s linear infinite alternate;
  }

  @keyframes shimmer {
    0% { opacity: 0.15; transform: rotate(0deg); }
    100% { opacity: 0.25; transform: rotate(360deg); }
  }

  /* CD label text */
  .label {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%) rotate(-15deg);
    text-align: center;
    font-size: 18px;
    color: #111;
    font-weight: 600;
    text-shadow: 0 1px 2px rgba(255, 255, 255, 0.5);
  }

  .label span {
    display: block;
    font-size: 12px;
    color: #333;
    font-weight: 400;
  }
</style>
</head>
<body>

<div class="cd">
  <div class="shine"></div>
  <div class="rainbow"></div>
  <div class="label">
    <br><span></span></span>
  </div>
</div>

</body>
</html>
