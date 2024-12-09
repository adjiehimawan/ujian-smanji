<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My WebView Website</title>
</head>
<body>
    <h1>Silahkan gunakan aplikasi CBT Exam Browser</h1>
    <script>
        function isAndroidWebView() {
    var userAgent = navigator.userAgent;
    return (userAgent.includes('wv') || userAgent.includes('WebView') || userAgent.includes('Android'));
}

function isMobile() {
    var userAgent = navigator.userAgent || navigator.vendor || window.opera;
    return (/android/i.test(userAgent) || /iPad|iPhone|iPod/.test(userAgent) && !window.MSStream);
}

if (!isAndroidWebView() && isMobile()) {
    alert("Aplikasi tidak bisa diakses via browser");
}

    </script>

</body>
</html>
