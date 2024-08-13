Seismic Event Prediction with CNN-LSTM

This project involves developing a predictive model for seismic events using a combination of Convolutional Neural Networks (CNN) and Long Short-Term Memory (LSTM) networks. 
The model is trained to predict the latitude, longitude, date (time until the next event), and magnitude of future seismic events based on historical earthquake data.

Dataset

The dataset used in this project consists of historical seismic event data from IGP. It includes the following key features:

	•	Date and Time: The exact date and time of each seismic event.
	•	Geographical Coordinates: Latitude and longitude of the event’s epicenter.
	•	Depth: The depth at which the event occurred.
	•	Magnitude: The magnitude of the seismic event.

The data was preprocessed to include additional features such as:

	•	Time Until Next Event: The time difference in hours until the next recorded event, used to predict the date of future events.
	•	Year, Month, Day, Hour, Minute, Second: Extracted from the event’s timestamp to enhance the model’s understanding of temporal patterns.

 Key Components:

	1.	Data Preparation:
	•	The dataset is processed to extract time-related features (year, month, day, hour, minute, second) and calculate the time until the next event.
	•	The data is then split into training and testing sets.
	2.	Model Architecture:
	•	A CNN-LSTM model is constructed to handle both spatial and temporal aspects of the data.
	•	The model outputs predictions for latitude, longitude, time until the next event, and magnitude.
	3.	Training:
	•	The model is trained using the prepared dataset, with the loss function based on Mean Squared Error (MSE).
	4.	Prediction and Evaluation:
	•	The model predicts the location, time, and magnitude of the next seismic event.
	•	Additional calculations are performed to assess the certainty of each prediction, providing a probability estimate for 
    the accuracy of the latitude, longitude, time, and magnitude predictions.

Results:
Predicted Latitude: -11.391161918640137
Predicted Longitude: -77.7036361694336
Predicted Date and Time of the next event: 2024-12-09 10:26:57.933060
Predicted Magnitude: 4.835737228393555
Predicted Latitude: -11.391161918640137 ± 4.5097002605573815 (Certainty: 77.43%)
Predicted Longitude: -77.7036361694336 ± 3.3862917397217807 (Certainty: 77.55%)
Predicted Date and Time of the next event: 2024-12-09 10:26:57.933060 ± 39.29922264497465 hours (Certainty: 96.41%)
Predicted Magnitude: 4.835737228393555 ± 0.465532616802117 (Certainty: 90.69%)

These coordinates point to a location near Huaral, a city in the Lima Region of Peru. Huaral is located about 75 kilometers north of Lima, the capital city of Peru. The region is situated relatively close to the Pacific coast and is known for its agricultural activities and proximity to the Andes mountains.

Given the coordinates, this area is within a seismically active region of Peru, which is part of the Pacific Ring of Fire, known for its frequent seismic activity.
