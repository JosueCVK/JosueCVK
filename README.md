<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Animated Flower</title>
<style>
  .flower {
    width: 100px;
    height: 100px;
    background: yellow;
    position: relative;
    border-radius: 50%;
    animation: bloom 3s infinite alternate;
  }
  .petal {
    width: 20px;
    height: 60px;
    background: pink;
    position: absolute;
    top: -30px;
    left: 40px;
    border-radius: 50%;
    transform-origin: center bottom;
    animation: swing 3s infinite alternate;
  }
  @keyframes bloom {
    from {
      width: 100px;
      height: 100px;
    }
    to {
      width: 120px;
      height: 120px;
    }
  }
  @keyframes swing {
    from {
      transform: rotate(0deg);
    }
    to {
      transform: rotate(20deg);
    }
  }
</style>
</head>
<body>
  <div class="flower">
    <div class="petal"></div>
    <div class="petal" style="transform: rotate(60deg);"></div>
    <div class="petal" style="transform: rotate(120deg);"></div>
    <div class="petal" style="transform: rotate(180deg);"></div>
    <div class="petal" style="transform: rotate(240deg);"></div>
    <div class="petal" style="transform: rotate(300deg);"></div>
  </div>
</body>
</html>
