# weather-app
Debugging the weather app

script.js:

line 3: ("search`)=>("#search"), wrong backticks`and missing selector syntax # (Prettier signaled undetermined string literal)
line 4: missing selector syntax #, spelling mistake query.Selectr
line 5: missing selector syntax #
line 6: missing selector syntax #
line 7: let temp = data.main.temp (In the OpenWeatherMap API response, the temperature is usually available in the main.temp property, not just temp)
line 19: tempEl.textContent = `${temp.toFixed(1)}°C` wrong type of "" => ``, I added .toFixed(2) to temp to round the temperature. (Chat GPT)
line 28: logical error => (temp < 0)
line 30: logical error => (temp <= 10)
line 32: logical error => (temp <= 20)
line 35: logical error => (temp > 20)
line 39: missing parenthesis around e => (e)
line 41: missing e at the begining of the line => e.preventDeafault() (Chat GPT)
