"#Flight-Price-Prediction" 

Overview
Data Description
train.csv
It contains the training data with flight details as described in the last section

Data Dictionary
Variable	Description
Airline	The name of the airline
source	The date of the journey
Destination	The destination where the service ends.
Route	The route taken by the flight to reach the destination.
Dep_Time	The time when the journey starts from the source
Arrival_Time	Time of arrival at the destination.
Duration	Total duration of the flight.
Total_Stops	Total stops between the source and destination.
Additional_Info	Additional information about the flight
Price	Target, The price of the ticket()
test.csv
It has flight details for which the participants are to submit the flight price

Evaluation Metric

Submissions are evaluated using the following metric(RMSE) between the predicted price(y_pred) and the observed price(y_true).:

-np.sqrt(np.square(np.log10(y_pred +1) - np.log10(y_true +1)).mean())
