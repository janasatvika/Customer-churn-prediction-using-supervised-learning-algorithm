# Customer-churn-prediction-using-supervised-learning-algorithm

![Logo](https://github.com/janasatvika/Customer-churn-prediction-using-supervised-learning-algorithm/blob/main/img%20assets/thumbnail.jpg)

<p>
The repository presented steps for building a model that predicted whether a customer would switch telecommunication service providers. The algorithms tested were Naive Bayes (NB), Decision Tree (DT), K-Nearest Neighbor (KNN), and Support Vector Machine (SVM). Two sets of data were provided: training data to train the model and test data to evaluate the model. The training data comprised 4250 rows with 20 columns. Out of a total of 4,250 samples, 3,652 (85.93%) belonged to the churn=no class, while 598 (14.07%) belonged to the churn=yes class. The test data comprised 750 rows with 20 columns, including the index of each sample and 19 features (excluding the target variable 'churn'). 
</p>

<h3>
  <span style='font-size:100px;'>&#128216;</span>
  Training Data Information
</h3>
<p>
  The training data was used to train the model.
</p>

<table>
  <tr>
    <th>Features</th>
    <th>Data type</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>state</td>
    <td>object</td>
    <td>Independent attribute</td>
  </tr>
  <tr>
    <td>account_length</td>
    <td>int64</td>
    <td>Independent attribute</td>
  </tr>
  <tr>
    <td>area_code</td>
    <td>object</td>
    <td>Independent attribute</td>
  </tr>
  <tr>
    <td>international_plan</td>
    <td>object</td>
    <td>Independent attribute</td>
  </tr>
  <tr>
    <td>voice_mail_plan</td>
    <td>object</td>
    <td>Independent attribute</td>
  </tr>
  <tr>
    <td>number_vmail_messages</td>
    <td>int64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_day_minutes</td>
    <td>float64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_day_calls </td>
    <td>int64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_day_charge</td>
    <td>float64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_eve_minutes</td>
    <td>float64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_eve_calls</td>
    <td>int64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_eve_charge</td>
    <td>float64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_night_minutes</td>
    <td>float64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_night_calls</td>
    <td>int64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_night_charge</td>
    <td>float64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_intl_minutes</td>
    <td>float64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_intl_calls</td>
    <td>int64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_intl_charge</td>
    <td>float64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>nnumber_customer_service_calls</td>
    <td>int64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>churn</td>
    <td>object</td>
    <td>Dependent attribute</td>
  </tr>
</table>

<h3>
  <span style='font-size:100px;'>&#128216;</span>
  Testing Data Information
</h3>
<p>
  The sample data was used to make predictions.
</p>

<table>
  <tr>
    <th>Features</th>
    <th>Data type</th>
    <th>Description</th>
  </tr>
    <tr>
    <td>id</td>
    <td>int64</td>
    <td>-</td>
  </tr>
  <tr>
    <td>state</td>
    <td>object</td>
    <td>Independent attribute</td>
  </tr>
  <tr>
    <td>account_length</td>
    <td>int64</td>
    <td>Independent attribute</td>
  </tr>
  <tr>
    <td>area_code</td>
    <td>object</td>
    <td>Independent attribute</td>
  </tr>
  <tr>
    <td>international_plan</td>
    <td>object</td>
    <td>Independent attribute</td>
  </tr>
  <tr>
    <td>voice_mail_plan</td>
    <td>object</td>
    <td>Independent attribute</td>
  </tr>
  <tr>
    <td>number_vmail_messages</td>
    <td>int64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_day_minutes</td>
    <td>float64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_day_calls </td>
    <td>int64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_day_charge</td>
    <td>float64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_eve_minutes</td>
    <td>float64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_eve_calls</td>
    <td>int64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_eve_charge</td>
    <td>float64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_night_minutes</td>
    <td>float64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_night_calls</td>
    <td>int64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_night_charge</td>
    <td>float64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_intl_minutes</td>
    <td>float64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_intl_calls</td>
    <td>int64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>total_intl_charge</td>
    <td>float64</td>
    <td>Independent attribute</td>
  </tr>
    <tr>
    <td>nnumber_customer_service_calls</td>
    <td>int64</td>
    <td>Independent attribute</td>
    </tr>
</table>

<h3>
  <span style='font-size:100px;'>&#9749;</span>
  Objective:
</h3>

<ul>
  <li>
    The method with the best performance was obtained.
  </li>
    <li>
    Predictions were made on the testing data.
  </li>
</ul>

<h3>
  References:
</h3>

<ul>
  <li>
    Kostas Diamantaras. (2020). Customer Churn Prediction 2020. Kaggle. https://kaggle.com/competitions/customer-churn-prediction-2020
  </li>
</ul>  
