<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>رسالة رومانسية</title>
  <style>
    body {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background: #ffe6f0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
    .envelope {
      width: 300px;
      height: 200px;
      background: #ffccd5;
      border-radius: 10px;
      position: relative;
      cursor: pointer;
      box-shadow: 0 5px 15px rgba(0,0,0,0.2);
      display: flex;
      justify-content: center;
      align-items: center;
      transition: transform 0.6s;
    }
    .envelope.open {
      transform: rotateX(180deg);
    }
    .message {
      display: none;
      position: absolute;
      top: 10px;
      left: 10px;
      right: 10px;
      bottom: 10px;
      background: #fff0f5;
      border-radius: 10px;
      padding: 20px;
      box-shadow: 0 5px 10px rgba(0,0,0,0.1);
      text-align: center;
      color: #b30059;
      font-size: 16px;
      line-height: 1.5;
    }
    .heart {
      color: #ff3366;
    }
  </style>
</head>
<body>

<div class="envelope" onclick="openEnvelope(this)">
  اضغط لفتح الظرف
  <div class="message">
    ادري تعبانه واعرف كلشي بس انتي احله ممرضه لا تخلين التعب يسيطر عليج استمري واني دائما وياج خطوه بخطوه ماعرف شكلج بس احبج هواي <span class="heart">🤍</span> وها ذكرت الابكوت و البروش مالتج حاضرات من هسه
  </div>
</div>

<script>
  function openEnvelope(el) {
    el.classList.toggle('open');
    const msg = el.querySelector('.message');
    if(msg.style.display === 'block') {
      msg.style.display = 'none';
    } else {
      msg.style.display = 'block';
    }
  }
</script>

</body>
</html>
