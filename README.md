# WeatherForecastAPI

### Abhishek Dhanasetty
I have four diffrent tabs named Historical, Forecast For A Particular Date, Forecast and Forecast Plots.

Forecast and Forecast Plots are dropdowns with values such as

* Forecast
	* From Database
	* From API (Weather Underground)
	
	
* Forecast Plots
	* From Database
	* From API (Weather Underground)
	
	
#### Working

* Historical

It returns a JSON string of daily.csv, which is stored in the sqlite database - daily.db


* Forecast For A Particular Date

It returns the TMAX and TMIN for a particular date stored in a database.

We enter the date between 20130101 to 20170209, in the input field FORMAT is **YYYYMMDD** on submit, it returns the **TMAX** and **TMIN** for that particlar date from the database.


* Forecast

It returns the TMAX and TMIN data for the next five days.

	* From Database
		It forecasts **TMAX** and **TMIN** data from the database for the next five days and a table is returned containing *DATE*, *TMAX*, and *TMIN*.
		
	* From API (Weather Underground)
		It forecasts **TMAX** and **TMIN** data for the next five days. It retreives information from Weather Underground API and a table is returned containing *DATE*, *TMAX*, and *TMIN*.
		
* Forecast Plots

It plots the forecasted values for the next five days.

	* From Database
		It plots **TMAX** and **TMIN** with date from the database for the next five days.
		
	* From API (Weather Underground)
		It plots **TMAX** and **TMIN** with date for the next five days. It retreives information from Weather Underground API.
		
