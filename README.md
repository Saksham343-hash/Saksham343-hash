- 👋 Hi, I’m @Saksham343-hash
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
function animateElement() {
    const elem = document.getElementById('your-element-id');
    let progress = 0;
    const duration = 1000; // Animation duration in milliseconds

    function animateFrame(timestamp) {
        const timeFraction = Math.min(1, (timestamp - startTime) / duration);
        progress = timeFraction;
        elem.style.width = progress * 100 + '%';

        if (timeFraction < 1) {
            requestAnimationFrame(animateFrame);
        }
    }

    const startTime = performance.now();
    requestAnimationFrame(animateFrame);
}

// Call the function to start the animation
animateElement();
<!---
Saksham343-hash/Saksham343-hash is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
