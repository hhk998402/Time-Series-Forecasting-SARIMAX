# Time-Series-Forecasting-SARIMAX
Using SARIMAX for Time Series Forecasting on Seasonal Data that is influenced by Exogenous variables

<h3 style="text-align:center">(Prepared for) Sangam 2019 - ML Hackathon by IITMAA</h3>
<p>
    <strong>Data Provided: </strong>Traffic Data (refer <code>train.csv</code> for more)
    <p><strong>Data description </strong></p>

<table>
	<tbody>
		<tr>
			<td>
			<p style="text-align: center;"><strong>Columns</strong></p>
			</td>
			<td>
			<p style="text-align: center;"><strong>Description</strong></p>
			</td>
		</tr>
		<tr>
			<td>
			<p>date_time</p>
			</td>
			<td>
			<p>Date, time, and hour of the data that is collected in the local IST time</p>
			</td>
		</tr>
		<tr>
			<td>
			<p>is_holiday</p>
			</td>
			<td>
			<p>Categorical Indian national holidays combined with regional holidays</p>
			</td>
		</tr>
		<tr>
			<td>
			<p>air_pollution_index</p>
			</td>
			<td>
			<p>Air Quality Index (10-300)</p>
			</td>
		</tr>
		<tr>
			<td>
			<p>humidity</p>
			</td>
			<td>
			<p>Numeric humidity in Celcius</p>
			</td>
		</tr>
		<tr>
			<td>
			<p>wind_speed</p>
			</td>
			<td>
			<p>Numeric wind speed in miles per hour</p>
			</td>
		</tr>
		<tr>
			<td>
			<p>wind_direction</p>
			</td>
			<td>
			<p>Cardinal wind direction (0-360 degree)</p>
			</td>
		</tr>
		<tr>
			<td>
			<p>visibility_in_miles</p>
			</td>
			<td>
			<p>Visibility of distance in miles</p>
			</td>
		</tr>
		<tr>
			<td>
			<p>dew_point</p>
			</td>
			<td>
			<p>Numeric dew point in Celcius</p>
			</td>
		</tr>
		<tr>
			<td>
			<p>temperature</p>
			</td>
			<td>
			<p>Numeric average temperature in Kelvin</p>
			</td>
		</tr>
		<tr>
			<td>
			<p>rain_p_h</p>
			</td>
			<td>
			<p>Numeric amount in mm of rain that occurred in the hour</p>
			</td>
		</tr>
		<tr>
			<td>
			<p>snow_p_h</p>
			</td>
			<td>
			<p>Numeric amount in mm of snow that occurred in the hour</p>
			</td>
		</tr>
		<tr>
			<td>
			<p>clouds_all</p>
			</td>
			<td>
			<p>Numeric percentage of cloud cover</p>
			</td>
		</tr>
		<tr>
			<td>
			<p>weather_type</p>
			</td>
			<td>
			<p>Categorical short textual description of the current weather</p>
			</td>
		</tr>
		<tr>
			<td>
			<p>weather_description</p>
			</td>
			<td>
			<p>Categorical longer textual description of the current weather</p>
			</td>
		</tr>
		<tr>
			<td>
			<p>traffic_volume</p>
			</td>
			<td>
			<p>Numeric hourly traffic volume bound in a specific direction</p>
			</td>
		</tr>
	</tbody>
</table>
The <code>traffic_volume</code> attribute has to be forecasted on the basis of the time series data provided, taking the exogenous variables into account
    <br><br>
    <strong>Approach used: </strong>SARIMAX (Seasonal Autoregressive Integrated Moving Average with eXogeneous variables)<br><br>
    <strong>Reason: </strong>The data provided is seasonal, and it is a time series data with multiple exogeneous variables influencing the result. Hence, the optimal statistical model that can be applied to this task is SARIMAX
    <br><br>
    <strong>Main Modules Used: </strong>
    <ul>
        <li><code>statsmodel</code> package in Python</li>
    </ul>
</p>
