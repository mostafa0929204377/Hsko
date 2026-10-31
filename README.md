# Hsko
حسكو الكباشي قنيط يحاا اثبات ذاته

<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>حسن الكباشي (حسكو)</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    body {
      background-color: #0f172a;
      color: #f8fafc;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      padding: 20px;
    }

    .container {
      background-color: #1e293b;
      border-radius: 16px;
      padding: 24px;
      max-width: 500px;
      width: 100%;
      box-shadow: 0 10px 25px rgba(0, 0, 0, 0.5);
      border: 1px solid #334155;
    }

    .profile-header {
      text-align: center;
      margin-bottom: 24px;
    }

    .profile-img {
      width: 130px;
      height: 130px;
      border-radius: 50%;
      object-fit: cover;
      border: 4px solid #38bdf8;
      box-shadow: 0 4px 10px rgba(56, 189, 248, 0.3);
      margin-bottom: 12px;
    }

    .profile-name {
      font-size: 1.5rem;
      font-weight: bold;
      color: #f1f5f9;
    }

    .profile-alias {
      font-size: 1rem;
      color: #94a3b8;
    }

    .tabs {
      display: flex;
      gap: 10px;
      margin-bottom: 20px;
    }

    .tab-btn {
      flex: 1;
      padding: 10px;
      border: none;
      border-radius: 8px;
      background-color: #334155;
      color: #e2e8f0;
      font-size: 0.95rem;
      cursor: pointer;
      font-weight: 600;
      transition: background 0.30s;
    }

    .tab-btn.active {
      background-color: #38bdf8;
      color: #0f172a;
    }

    .tab-content {
      display: none;
      animation: fadeIn 0.3s ease-in-out;
    }

    .tab-content.active {
      display: block;
    }

    .list {
      list-style: none;
    }

    .list-item {
      background-color: #0f172a;
      padding: 12px 16px;
      border-radius: 8px;
      margin-bottom: 10px;
      border-right: 4px solid #38bdf8;
      font-size: 0.95rem;
      line-height: 1.5;
    }

    .flaws .list-item {
      border-right-color: #f43f5e;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(5px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>

  <div class="container">
    <div class="profile-header">
      <img src="https://cdn.phototourl.com/member/2026-10-31-606c7cf3-4599-4176-82ac-406c5b990e8b.jpg" alt="حسن الكباشي" class="profile-img" onerror="this.src='https://via.placeholder.com/130?text=حسكو'">
      <h1 class="profile-name">حسن الكباشي</h1>
      <p class="profile-alias">الشهير بـ "حسكو"</p>
    </div>

    <div class="tabs">
      <button class="tab-btn active" onclick="switchTab('facts', this)">حقائق عن حسكو</button>
      <button class="tab-btn" onclick="switchTab('flaws', this)">عيوب وملاحظات</button>
    </div>

    <!-- قسم الحقائق -->
    <div id="facts" class="tab-content active">
      <ul class="list">
        <li class="list-item">صانع محتوى غير رائج على التيك توك.</li>
        <li class="list-item">شغال في الدهب، لكن الحالة المادية مفلسة دائماً.</li>
        <li class="list-item">بيحاول يجذب المتابعين بصوره بس الحظ معانده.</li>
      </ul>
    </div>

    <!-- قسم العيوب والملاحظات -->
    <div id="flaws" class="tab-content flaws">
      <ul class="list">
        <li class="list-item">قنيط شديد.</li>
        <li class="list-item">مفروض يعتزل التيك توك.</li>
        <li class="list-item">مفروض يعتزل الرومات.</li>
      </ul>
    </div>
  </div>

  <script>
    function switchTab(tabId, element) {
      document.querySelectorAll('.tab-content').forEach(content => {
        content.classList.remove('active');
      });
      document.querySelectorAll('.tab-btn').forEach(btn => {
        btn.classList.remove('active');
      });

      document.getElementById(tabId).classList.add('active');
      element.classList.add('active');
    }
  </script>

</body>
</html>
