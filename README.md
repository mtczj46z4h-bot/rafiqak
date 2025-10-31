<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>تقييم حالتك المزاجية - رفيقك</title>
  <style>
    body {
      font-family: 'Cairo', sans-serif;
      background-color: #f5f8ff;
      color: #333;
      text-align: center;
      padding: 40px;
    }
    h1 { color: #3b5998; }
    button {
      background-color: #5a7ce2;
      color: white;
      border: none;
      padding: 12px 20px;
      margin: 10px;
      border-radius: 10px;
      font-size: 16px;
      cursor: pointer;
    }
    button:hover { background-color: #3b5998; }
    #result {
      margin-top: 30px;
      font-size: 20px;
      color: #444;
    }
  </style>
</head>
<body>
  <h1>تقييم حالتك المزاجية</h1>
  <p>كيف تشعر اليوم؟</p>
  
  <button onclick="showMessage('سعيد')">سعيد 😊</button>
  <button onclick="showMessage('محايد')">محايد 😐</button>
  <button onclick="showMessage('حزين')">حزين 😔</button>

  <div id="result"></div>

  <script>
    function showMessage(mood) {
      let message = "";
      if (mood === 'سعيد') message = "رائع! استمر في نشر طاقتك الإيجابية 🌟";
      else if (mood === 'محايد') message = "خذ لحظة للراحة والتأمل، ربما فنجان قهوة يساعد ☕";
      else if (mood === 'حزين') message = "تذكر أن المشاعر المؤلمة مؤقتة، أنت أقوى مما تظن 💪";
      document.getElementById('result').innerText = message;
    }
  </script>

  <p><a href="index.html">⬅ العودة إلى الصفحة الرئيسية</a></p>
</body>
</html>
