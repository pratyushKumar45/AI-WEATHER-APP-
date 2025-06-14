<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Weather-App</title>
</head>
<style>
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    border: none;
    outline: none;
    font-family: sans-serif;
}

body{
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: black;
}

.container{
    width: 400px;
    height: min-content;
    background-color: white;
    border-radius: 12px;
    padding: 20px;
}

.search-box{
    width: 100%;
    height: min-content;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.search-box input{
    width: 84%;
    font-size: 20px;
    text-transform: capitalize;
    color: black;
    background-color: #e6f5fb;
    padding: 12px 16px;
    border-radius: 14px;
}

.search-box input::placeholder{
    color: black;
}

.search-box button{
    width: 46px;
    height: 46px;
    background-color: #e6f5fb;
    border-radius: 50%;
    cursor: pointer;
    font-size: 20px;
}

.search-box button:hover{
    color: #fff;
    background-color: #ababab;
}

.weather-body{
    justify-content: center;
    align-items: center;
    flex-direction: column;
    margin-block: 20px;
    display: none;
}

.weather-body img{
    width: 60%;
}

.weather-box{
    margin-block: 20px;
    text-align: center;
}

.weather-box .temperature{
    font-size: 40px;
    font-weight: 800;
    position: relative;
}

.weather-box .temperature sup{
    font-size: 20px;
    position: absolute;
    font-weight: 600;
}

.weather-box .description{
    font-size: 20px;
    font-weight: 700;
    text-transform: capitalize;
}

.weather-details{
    width: 100%;
    display: flex;
    justify-content: space-between;
    margin-top: 30px;
}

.humidity, .wind{
    display: flex;
    align-items: center;
}

.humidity{
    margin-left: 20px;
}

.wind{
    margin-right: 20px;
}

.weather-details i{
    font-size: 36px;
}

.weather-details .text{
    margin-left: 10px;
    font-size: 16px;
}

.text span{
    font-size: 20px;
    font-weight: 700;
}

.location-not-found{
    margin-top: 20px;
    display: none;
    align-items: center;
    justify-content: center;
    flex-direction: column;
}

.location-not-found h1{
    font-size: 20px;
    color: #6b6b6b;
    margin-block-end: 15px;
}

.location-not-found img{
    width: 80%;
}
<style>
<body>
    <div class="container">
        <div class="header">
            <div class="search-box">
                <button class="fa-solid fa-location-dot" id="get-location"></button>
                <input type="text" placeholder="Enter Your Location" class="input-box">
                <button class="fa-solid fa-magnifying-glass" id="searchBtn"></button>
            </div>
        </div>
        <div class="location-not-found">
            <h1>Sorry, Location not found!!!</h1>
            <img src="Pictures/404.png" alt="404 Error">
        </div>
        <div class="weather-body">
            <img src="Pictures/clear.png" alt="Weather Image" class="weather-img">
            <div class="weather-box">
                <p class="temperature">0<sup>°C</sup></p>
                <p class="description">light rain</p>
            </div>
            <div class="wether-details">
                <div class="humidity">
                    <i class="fa-sharp fa-solid fa-droplet"></i>
                    <div class="text">
                        <span id="humidity">45%</span>
                        <p>Humidity</p>
                    </div>
                </div>
                <div class="wind">
                    <i class="fa-solid fa-wind"></i>
                    <div class="text">
                        <span id="wind-speed">12Km/H</span>
                        <p>Wind Speed</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!--Script-->
    <script src="script.js"></script>
    <script src="https://kit.fontawesome.com/92e8221daa.js" crossorigin="anonymous"></script>
</body>
</html>
