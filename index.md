---
layout: default
---

# beer.app

Bestätigen Sie, dass Sie ein Mensch sind, indem Sie die Aktion unten ausführen.

<noscript><p>Enable JavaScript and cookies to continue</p></noscript>

<div class="i-captcha" style="margin-bottom: 20px;"></div>

beer.app muss die Sicherheit Ihrer Verbindung überprüfen, bevor Sie fortfahren können.

<div class="reqid"></div>

<script src="https://brandondong.github.io/impossible-captchas/api/build/captcha.js"></script>
<script>
(function () {
  'use strict';
  
  function main() {
    const reqids = document.getElementsByClassName("reqid");
    for (const elem of reqids) {
      const p = document.createElement("p");
      const reqid = Math.random().toString(16).slice(2)  
      p.innerHTML = "Request ID: " + reqid
      elem.appendChild(p)
    }
  }

  // Taken from https://developer.mozilla.org/en-US/docs/Web/Events/DOMContentLoaded#Checking_whether_loading_is_already_complete.
  if (document.readyState === "loading") {  // Loading hasn't finished yet
    document.addEventListener("DOMContentLoaded", main);
  } else {  // `DOMContentLoaded` has already fired
    main();
  }

}());
</script>
