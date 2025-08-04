<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Redirecting...</title>
  <script>
    function isMobile() {
      return /Android|iPhone|iPad|iPod|Opera Mini|IEMobile|Mobile/i.test(navigator.userAgent);
    }

    function getNextOfferIndex(offersLength) {
      const timestamp = Date.now();
      return timestamp % offersLength;
    }

    window.onload = function () {
      const offers = [
        "https://grzvkg.amurllove.com/?utm_source=da57dc555e50572d&ban=tiktok&j1=1&s1=212364&s2=2140295",
        "https://snurik.top/click?o=2&a=6549&sub_id1=tt",
        "https://prev.affomelody.com/fFVv28"
      ];

      const desktopRedirect = "https://www.instagram.com/";
      const finalUrl = isMobile()
        ? offers[getNextOfferIndex(offers.length)]
        : desktopRedirect;

      setTimeout(() => {
        window.location.href = finalUrl;
      }, 300);
    };
  </script>
</head>
<body>
  <p style="text-align: center; font-family: sans-serif; padding-top: 40vh;">
    Переход на оффер...
  </p>
</body>
</html>
