# Vidizayn - Vistream website with HTML, CSS & JS

## DEMO
![vistream](https://user-images.githubusercontent.com/101663533/189988458-53668ed7-dcdf-46a0-b2eb-87711fc88b2a.png)

## JS Countdown
![Vistream](https://user-images.githubusercontent.com/101663533/189989505-c7e52794-3297-4c62-a86a-1a604231c08c.gif)

### Countdown Code
`const countdown = () => {
    const countDate = new Date('November 29, 2022 00:00:00').getTime();
    const now = new Date().getTime();
    const gap = countDate - now;

    // Time
    const second = 1000;
    const minute = second * 60;
    const hour = minute * 60;
    const day = hour * 24;

    //Calculate
    const textDay = Math.floor(gap / day);
    const textHour = Math.floor((gap % day) / hour);
    const textMinute = Math.floor((gap % hour) / minute);
    const textSecond = Math.floor((gap % minute) / second);
    
    document.querySelector('.day').innerText = textDay;
    document.querySelector('.hour').innerText = textHour;
    document.querySelector('.minute').innerText = textMinute;
    document.querySelector('.second').innerText = textSecond;
};
setInterval(countdown, 1000);`
