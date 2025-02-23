# Hafez_Fal
<!DOCTYPE html><html lang="fa">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>فال حافظ</title>
    <style>
        body {
            font-family: Tahoma, sans-serif;
            text-align: center;
            background-color: #ffebcd;
        }
        .container {
            max-width: 600px;
            margin: 50px auto;
            padding: 20px;
            background: #fff;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
        }
        button {
            padding: 10px 20px;
            font-size: 18px;
            background-color: #ff5722;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background-color: #e64a19;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>فال حافظ</h1>
        <img src="https://upload.wikimedia.org/wikipedia/commons/5/5b/Hafez.jpg" alt="حافظ" width="200">
        <p id="poem">برای گرفتن فال روی دکمه کلیک کنید.</p>
        <p id="meaning"></p>
        <button onclick="getRandomPoem()">فال بگیر</button>
        <h3>سال ۱۴۰۴ مبارک!</h3>
    </div><script>
    const poems = [
        {verse: "صلاح کار کجا و من خراب کجا / ببین تفاوت ره کز کجاست تا به کجا", meaning: "بهتر است بدانیم که چه چیزی برای ما خوب است و چه چیزی به صلاح نیست، زیرا مسیر درست و نادرست بسیار متفاوت‌اند."},
        {verse: "ما آزموده‌ایم در این شهر بخت خویش / بیرون کشید باید از این ورطه رخت خویش", meaning: "اگر شرایط نامناسب است، بهتر است خود را از آن وضعیت خارج کنیم."},
        {verse: "حجاب چهره جان می‌شود غبار تنم / خوشا دمی که از آن چهره پرده برفکنم", meaning: "جسم، مانع درک حقیقت روح است و خوشا آن لحظه‌ای که بتوان پرده از حقیقت برداشت."},
        {verse: "سال‌ها دل طلب جام جم از ما می‌کرد / آنچه خود داشت ز بیگانه تمنا می‌کرد", meaning: "گاهی انسان در جستجوی چیزی است که در درون خود دارد اما از دیگران طلب می‌کند."},
        {verse: "چو بشنوی سخن اهل دل مگو که خطاست / سخن‌شناس نه‌ای جان من خطا این جاست", meaning: "هر سخنی را نباید به سادگی رد کرد، بلکه باید با دقت و تفکر به آن گوش داد."},
        {verse: "زاهد ار رندی حافظ نکند فهم چه شد / دیو بگریزد از آن قوم که قرآن خوانند", meaning: "اگر شخصی نتواند معنای عمیق زندگی را درک کند، مشکلی نیست، زیرا حقیقت برای اهل آن روشن است."},
        // ادامه ۶۴ شعر دیگر...
    ];

    function getRandomPoem() {
        let randomIndex = Math.floor(Math.random() * poems.length);
        document.getElementById("poem").innerText = poems[randomIndex].verse;
        document.getElementById("meaning").innerText = poems[randomIndex].meaning;
    }
</script>

</body>
</html>
