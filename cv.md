# Evgeniy Chernyavskiy

## My contacts :
**Phone** : *+375292547610;*
**Mail** : *lognard1994@gmail.com;*

## About me
I am 27 years old. I want to change my current place of work.
I decided to try myself in the IT field.
Web development is very interesting.
I have no experience in this field, expect for solving small tasks in JavaScript,
a handful of pages based on layouts.

## Skills
* *JavaScript* 
* *HTML*
* *CSS*
* *Bootstrap*
* *git*
* *react (theory)*

## Example code javaScript
```javascript
function slider(){
    let indexSlider = 1,
    slidePhoto = document.querySelectorAll('.slider-item'),
    prev = document.querySelector('.prev'),
    next = document.querySelector('.next'),
    slidedots = document.querySelector('.slider-dots'),
    dots = document.querySelectorAll('.dot');
    console.log(dots.length);
    
    showSlide(indexSlider);
    function showSlide(n){
        if (n > slidePhoto.length){
            indexSlider = 1;
        }
        if (n < 1){
            indexSlider = slidePhoto.length
        }
        slidePhoto.forEach((item)=> item.style.display = 'none');
        dots.forEach((item)=> item.classList.remove('dot-active'));

        slidePhoto[indexSlider - 1].style.display = 'block';
        dots[indexSlider - 1].classList.add('dot-active');
    }

   function plusSlide(n){
        showSlide(indexSlider += n)
   }
    function currentSlide(n){
            showSlide(indexSlider = n)
        }
   
   prev.addEventListener('click' , function(){
        plusSlide(-1)
    });
    next.addEventListener('click' , function(){
        plusSlide(1);
    })

    slidedots.addEventListener('click' , function(event){
        for (let i = 0; i < dots.length; i++){
            if (event.target.classList.contains('dot') && event.target == dots[i]){
                currentSlide(i+1);
            }
        }
    });
}
};
```
## Work experience
Trainings from **Glo-academy**, online lectures, adding functionality on page using JavaScript.

## Education 
I graduated from the Belarusian National Technical University in 2016.
Faculty of Information Technologies and Robotics.
FrontEnd - self-education.

# English level
A2.
