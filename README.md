# A_WEATHER_APPLICATION
# Django Weather Application

A modern, responsive weather application built with Django that allows users to search for real-time weather information for cities around the world.

![Django Weather App](https://source.unsplash.com/800x400/?weather)

## Features

- **Real-time Weather Data**: Fetches up-to-date weather information using OpenWeatherMap API
- **City Search**: Look up weather in any city worldwide
- **Recent Searches**: Keeps track of your recent searches for quick access
- **Responsive Design**: Works on desktop and mobile devices
- **Error Handling**: Graceful handling of API errors and invalid city names

## Technology Stack

- **Backend**: Python 3.8+ & Django 4.2+
- **Frontend**: HTML, CSS, Bootstrap 5
- **API**: OpenWeatherMap
- **Database**: SQLite (default Django database)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/GDIAMEL/A_WEATHER_APPLICATION.git
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Get an API key from [OpenWeatherMap](https://openweathermap.org/api)

5. Create a `.env` file in the project root:
```
OPENWEATHERMAP_API_KEY=your_api_key_here
```

6. Apply migrations:
```bash
python manage.py migrate
```

7. Run the development server:
```bash
python manage.py runserver
```

8. Visit http://127.0.0.1:8000/ in your browser to use the app.

## Project Structure

```
weather_project/
├── manage.py
├── weather_project/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
└── weather_app/
    ├── __init__.py
    ├── admin.py
    ├── apps.py
    ├── forms.py
    ├── migrations/
    ├── models.py
    ├── static/
    │   └── css/
    │       └── style.css
    ├── templates/
    │   └── weather_app/
    │       ├── base.html
    │       ├── index.html
    │       └── weather.html
    ├── tests.py
    ├── urls.py
    └── views.py
```

## Usage

1. Enter a city name in the search box
2. Click "Search" to get the current weather
3. View weather details including temperature, description, humidity, and wind speed
4. Use the "Search Again" button to look up another city
5. Your recent searches will appear on the home page for quick access

## Screenshots

![Home Page](https://source.unsplash.com/400x300/?app)
![Weather Results](https://source.unsplash.com/400x300/?forecast)

## Future Enhancements

- User authentication to save favorite cities
- 5-day weather forecast
- Geolocation to automatically detect user's city
- More detailed weather information
- Dark mode toggle

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- OpenWeatherMap for providing the weather data API
- Bootstrap for the responsive design components
