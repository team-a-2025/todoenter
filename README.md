<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Todoapp</title>
</head>
</header>
<body>
    <main>
        <!-- 入力フォーム -->
        <form action="#" id="form">
            <input type="text" name="content">
            <input type="submit" value="送信">
        </form>
        <!-- 入力結果を出力 -->
        <p id="output"></p>
    </main>
</body>
<!-- 以下JavaScriptを記述 -->
<script>
    // submit時にイベント実行をする関数
    document.getElementById('form').onsubmit = function (event) {
        // 再読み込み防止
        event.preventDefault();
        // 入力フォームの内容を取得
        let inputForm = document.getElementById('form').content.value;
		// 入力内容を画面に出力
        document.getElementById('output').textContent = `${inputForm}`;
    }
</script>
</html>
