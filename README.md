<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<title>محرر أكواد - تجربة البرمجة</title>
<style>
  body {
    margin: 0;
    font-family: Arial, sans-serif;
    background-color: #f5f6fa;
    display: flex;
    flex-direction: column;
    height: 100vh;
  }

  header {
    background-color: #3498db;
    color: white;
    padding: 15px;
    text-align: center;
    font-size: 24px;
  }

  main {
    flex: 1;
    display: flex;
    gap: 10px;
    padding: 10px;
  }

  textarea {
    width: 50%;
    height: 100%;
    font-family: monospace;
    font-size: 16px;
    padding: 10px;
    border-radius: 5px;
    border: 1px solid #ccc;
    resize: none;
    background-color: #f0f8ff;
  }

  iframe {
    width: 50%;
    height: 100%;
    border: 1px solid #ccc;
    border-radius: 5px;
    background-color: white;
  }

  button {
    background-color: #2ecc71;
    color: white;
    border: none;
    padding: 10px 15px;
    margin: 10px;
    font-size: 16px;
    cursor: pointer;
    border-radius: 5px;
  }

  button:hover {
    background-color: #27ae60;
  }

</style>
</head>
<body>

<header>محرر أكواد - تجربة البرمجة</header>

<main>
  <textarea id="codeArea">
<!DOCTYPE html>
<html>
<head>
  <title>صفحة جديدة</title>
</head>
<body>
  <h1>مرحباً بك في تجربة البرمجة!</h1>
  <p>اكتب كودك هنا وجربه.</p>
</body>
</html>
  </textarea>
  <iframe id="preview"></iframe>
</main>

<button onclick="runCode()">تشغيل الكود</button>

<script>
function runCode() {
  let code = document.getElementById('codeArea').value;
  let iframe = document.getElementById('preview');
  iframe.srcdoc = code;
}
</script>

</body>
</html>
