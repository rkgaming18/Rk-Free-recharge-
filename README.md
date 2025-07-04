<script>
  const wheel = document.querySelector('.wheel');
  const spinBtn = document.querySelector('.spinBtn');
  const shareBtn = document.querySelector('.shareBtn');
  const instaBtn = document.querySelector('.instaBtn');
  const resultBox = document.createElement('div');
  document.body.appendChild(resultBox);

  const prizes = ["২৯৯ Jio Recharge", "১GB Data", "৫GB Data", "২GB Data"];
  const INSTAGRAM_USERNAME = "akhim_b18"; // ← তোমাৰ IG username

  spinBtn.addEventListener('click', () => {
    spinBtn.disabled = true;
    const deg = Math.floor(5000 + Math.random() * 5000);
    wheel.style.transition = "transform 5s ease-out";
    wheel.style.transform = `rotate(${deg}deg)`;

    setTimeout(() => {
      const selectedIndex = Math.floor(((deg % 360) / 90));
      const selectedPrize = prizes[3 - selectedIndex]; // Clockwise 0 = last item
      resultBox.innerHTML = `
        <h2 style="color:white;">আপুনি জিকিলে: ${selectedPrize}</h2>
        <a class="shareBtn" href="#" target="_blank">📤 WhatsAppত Share কৰক</a>
        <a class="instaBtn" href="https://instagram.com/${INSTAGRAM_USERNAME}" target="_blank">📷 Instagram Follow কৰক</a>
      `;
      resultBox.style.marginTop = "20px";
      resultBox.style.display = "flex";
      resultBox.style.flexDirection = "column";
      resultBox.style.alignItems = "center";

      // WhatsApp Share Button Functionality
      const shareBtn = resultBox.querySelector(".shareBtn");
      shareBtn.addEventListener("click", () => {
        const shareText = encodeURIComponent(`নমস্কাৰ! মই RK Gaming Spin ৰ পৰা ${selectedPrize} জিকিলো। আপুনিও ঘূৰাই চাওক! 👉 https://rkgaming18.github.io/Rk-Free-recharge-/`);
        shareBtn.href = `https://wa.me/?text=${shareText}`;
      });

    }, 5200);
  });
</script>
