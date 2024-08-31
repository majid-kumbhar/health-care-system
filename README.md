
---

# Disease Prediction Web Application

This Flask application predicts diseases based on the symptoms entered by the user. It uses a pre-trained model to classify the disease and provides recommendations on precautions, medications, diets, and workouts related to the predicted disease.

## Project Structure

- `app.py`: The main Flask application file.
- `dataset/`: Directory containing CSV files with disease-related data.
- `model/`: Directory containing the saved model (`svc.pkl`).
- `templates/`: Directory containing HTML templates for the web interface.
- `requirements.txt`: File listing the required Python packages.


## Data

The application requires the following datasets to be placed in the `dataset/` directory:

- `symtoms_df.csv`: A CSV file with symptom data.
- `precautions_df.csv`: A CSV file with precautionary measures.
- `workout_df.csv`: A CSV file with workout recommendations.
- `description.csv`: A CSV file with disease descriptions.
- `medications.csv`: A CSV file with medication recommendations.
- `diets.csv`: A CSV file with diet recommendations.

The model file (`svc.pkl`) should be placed in the `model/` directory.

## How to Run

1. Navigate to the project directory.

2. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the Flask application:

   ```bash
   python app.py
   ```

4. Open your web browser and go to `http://127.0.0.1:5000/` to access the application.

## Endpoints

- `/`: The home page where users can enter symptoms.
- `/predict`: A POST route to submit symptoms and get predictions.
- `/about`: Information about the application.
- `/contact`: Contact information.
- `/developer`: Information about the developer.
- `/blog`: Blog or additional information related to the application.

## Notes

- Ensure that the paths to the dataset files and the model are correct.
- The application is set to run in debug mode. For production use, change the `debug` parameter to `False` in the `app.run()` method.
