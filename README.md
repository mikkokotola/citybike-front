# Citybike-front
Citybike predictor app frontend.

### Related repositories
[Backend](https://github.com/juhapekkamoilanen/citybike-statistical-analysis) for the citybike predictor app is a separate repository.

### Deployment
NOTE: as of 4.1.2020, the backend is not functional in historical mode due to the unavailability of historical citybike availability data from HSL at https://dev.hsl.fi/citybike/stations/. The app will be in summer mode until further notice.

Frontend is deployed at [https://citybike-pred.herokuapp.com/](https://citybike-pred.herokuapp.com/). The frontend uses the python backend deployed at [https://citybike-helsinki-predictor.herokuapp.com/](https://citybike-helsinki-predictor.herokuapp.com/).

### Frontend info
The frontend is vanilla JS and uses [D3.js](https://d3js.org/). For heroku deployment it is set up as a fake PHP app.

# Development

### Frontend

1. Go to frontend repository root and start a local webserver to serve html and js files

```
python3 -m http.server
```

2. Open browser from localhost:8000
3. Click on home.html

NOTE: the frontend uses the Heroku-deployed backend. If you want to use a locally run backend, change the first line in js-src/plotter.js to const baseUrl = 'http://localhost:3001'
