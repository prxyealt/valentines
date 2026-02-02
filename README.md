@@ -133,7 +133,7 @@
  <canvas id="confettiCanvas"></canvas>

  <main class="card">
    <!-- ORIGINAL CUTE ANIMAL WITH HEART -->
    <!-- ANIMAL WITH HEART -->
    <svg class="art" viewBox="0 0 320 240" xmlns="http://www.w3.org/2000/svg">
      <defs>
        <linearGradient id="fur" x1="0" x2="1">
@@ -178,7 +178,7 @@ <h1>my love, will you be my valentine?</h1>
      <button id="noBtn">No</button>
    </section>

    <!-- HINT (ONLY FIRST SECTION) -->
    <!-- HINT -->
    <div class="hint" id="hint">“No” seems a bit shy 😈</div>

    <section class="result" id="result">
@@ -198,7 +198,7 @@ <h2>YAY! 🎉</h2>
    const result = document.getElementById("result");
    const hint = document.getElementById("hint");

    /* ---------- CONFETTI (FIXED FULL SCREEN) ---------- */
    /* ---------- CONFETTI ---------- */
    const confettiCanvas = document.getElementById("confettiCanvas");

    function resizeConfettiCanvas() {
@@ -292,7 +292,7 @@ <h2>YAY! 🎉</h2>
    /* ---------- YES CLICK ---------- */
    yesBtn.addEventListener("click", () => {
      zone.style.display = "none";
      hint.style.display = "none";     // ✅ HIDE THE HINT
      hint.style.display = "none";     // HIDE THE HINT
      result.style.display = "block";
      resizeConfettiCanvas();
      fullScreenConfetti();
@@ -302,3 +302,4 @@ <h2>YAY! 🎉</h2>
</html>
