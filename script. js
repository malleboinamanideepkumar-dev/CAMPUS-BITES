/* ===========================================
   CAMPUS BITES PREMIUM WEBSITE
   script.js
=========================================== */

// ===============================
// Loader
// ===============================

window.addEventListener("load", () => {

    const loader = document.getElementById("loader");

    if (loader) {

        loader.style.opacity = "0";

        loader.style.visibility = "hidden";

        setTimeout(() => {

            loader.remove();

        }, 800);

    }

});

// ===============================
// Sticky Header
// ===============================

const header = document.querySelector("header");

window.addEventListener("scroll", () => {

    if (window.scrollY > 80) {

        header.classList.add("sticky");

    } else {

        header.classList.remove("sticky");

    }

});

// ===============================
// Smooth Scroll
// ===============================

document.querySelectorAll('a[href^="#"]').forEach(link => {

    link.addEventListener("click", function(e) {

        e.preventDefault();

        const target = document.querySelector(this.getAttribute("href"));

        if (target) {

            target.scrollIntoView({

                behavior: "smooth"

            });

        }

    });

});

// ===============================
// Scroll Reveal
// ===============================

const revealElements = document.querySelectorAll(

".food-card,.why-card,.contact-card,.experience,.franchise-box,.section-title"

);

const revealOnScroll = () => {

    revealElements.forEach(el => {

        const top = el.getBoundingClientRect().top;

        if (top < window.innerHeight - 120) {

            el.classList.add("show");

        }

    });

};

window.addEventListener("scroll", revealOnScroll);

revealOnScroll();
// ===============================
// Active Navigation Highlight
// ===============================

const sections = document.querySelectorAll("section");
const navLinks = document.querySelectorAll("nav ul li a");

window.addEventListener("scroll", () => {

    let current = "";

    sections.forEach(section => {

        const sectionTop = section.offsetTop - 120;

        if (window.scrollY >= sectionTop) {

            current = section.getAttribute("id");

        }

    });

    navLinks.forEach(link => {

        link.classList.remove("active");

        if (link.getAttribute("href") === "#" + current) {

            link.classList.add("active");

        }

    });

});

// ===============================
// Hero Fade Animation
// ===============================

const heroContent = document.querySelector(".hero-content");

window.addEventListener("scroll", () => {

    if (!heroContent) return;

    const offset = window.scrollY;

    heroContent.style.opacity = Math.max(1 - offset / 500, 0);

    heroContent.style.transform =
        `translateY(calc(-50% + ${offset * 0.25}px))`;

});

// ===============================
// Food Card Hover Effect
// ===============================

document.querySelectorAll(".food-card").forEach(card => {

    card.addEventListener("mouseenter", () => {

        card.style.transform = "translateY(-12px) scale(1.02)";

    });

    card.addEventListener("mouseleave", () => {

        card.style.transform = "";

    });

});

// ===============================
// Contact Card Hover
// ===============================

document.querySelectorAll(".contact-card").forEach(card => {

    card.addEventListener("mouseenter", () => {

        card.style.boxShadow =
            "0 20px 40px rgba(255,180,0,.25)";

    });

    card.addEventListener("mouseleave", () => {

        card.style.boxShadow = "";

    });

});

// ===============================
// Footer Year
// ===============================

const yearElement = document.getElementById("year");

if (yearElement) {

    yearElement.textContent = new Date().getFullYear();

}
// ===============================
// Back To Top Button
// ===============================

const backToTop = document.createElement("button");

backToTop.innerHTML = "↑";

backToTop.id = "backToTop";

document.body.appendChild(backToTop);

Object.assign(backToTop.style, {
    position: "fixed",
    right: "25px",
    bottom: "25px",
    width: "50px",
    height: "50px",
    borderRadius: "50%",
    border: "none",
    background: "#ffb400",
    color: "#111",
    fontSize: "22px",
    fontWeight: "bold",
    cursor: "pointer",
    display: "none",
    zIndex: "9999",
    transition: "0.3s"
});

window.addEventListener("scroll", () => {

    if (window.scrollY > 400) {

        backToTop.style.display = "block";

    } else {

        backToTop.style.display = "none";

    }

});

backToTop.addEventListener("click", () => {

    window.scrollTo({

        top: 0,

        behavior: "smooth"

    });

});

// ===============================
// Button Click Animation
// ===============================

document.querySelectorAll(".gold-btn,.outline-btn,.nav-btn").forEach(btn => {

    btn.addEventListener("click", function () {

        this.style.transform = "scale(0.96)";

        setTimeout(() => {

            this.style.transform = "";

        }, 150);

    });

});

// ===============================
// Image Fade In
// ===============================

document.querySelectorAll("img").forEach(img => {

    img.addEventListener("load", () => {

        img.style.opacity = "1";

    });

});

// ===============================
// Console Message
// ===============================

console.log("%cCampus Bites Website Loaded Successfully!",
"color:#ffb400;font-size:18px;font-weight:bold;");

console.log("Developed for Campus Bites");

// ===============================
// End
// ===============================
