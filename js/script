// Your API key here (replace this string)
const API_KEY = 'f15dfb670f87f97aa95093274121d725';

// DOM elements
const cityInput = document.getElementById('cityInput');
const searchBtn = document.getElementById('searchBtn');
const currentDiv = document.getElementById('currentWeather');

// Event listener (we'll talk about this on roadmap "Functions & Events")
searchBtn.addEventListener('click', () => {
  const city = cityInput.value.trim();
  if (city) {
    getCurrentWeather(city);
  }
});

// Function to fetch weather
async function getCurrentWeather(city) {
  const url = `https://api.openweathermap.org/data/2.5/weather?q=${city}&appid=${API_KEY}&units=metric`;

  try {
    const response = await fetch(url);
    const data = await response.json();
    
    console.log('API Response:', data);   // ← Look at this in console!
    // We'll display it next

  } catch (error) {
    console.error('Error fetching weather:', error);
  }
}