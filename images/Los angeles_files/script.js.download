let slideIndex = 0; 
showSlides(slideIndex);

function currentSlide(n) {
    showSlides(slideIndex = n); 
}

function showSlides(n) {
    let i;
    const slides = document.querySelectorAll(".carousel-item");
    const dots = document.querySelectorAll(".dot");
    
    for (i = 0; i < slides.length; i++) {
        slides[i].style.display = "none";
    }
    
    for (i = 0; i < dots.length; i++) {
        dots[i].classList.remove("active");
    }
    
    if (n < 0) { 
        slideIndex = slides.length - 1; 
    } else if (n >= slides.length) { 
        slideIndex = 0; 
    } else { 
        slideIndex = n; 
    }
    slides[slideIndex].style.display = "block";
    dots[slideIndex].classList.add("active");
}

const dotButtons = document.querySelectorAll(".dot");
dotButtons.forEach((dot, index) => {
    dot.addEventListener("click", () => {
        currentSlide(index);
    });
});

const imageButtons = document.querySelectorAll(".carousel-item img");
imageButtons.forEach((image, index) => {
    image.addEventListener("click", () => {
        currentSlide(index);
    });
});