Sure! After splitting your data and training the model (as shown earlier), the next step is testing the model and making predictions on new data.

Here's how you can do it:


---

✅ Continue From Trained Model

Assume you've already done this:

# Model already trained
model.fit(X_train, y_train)


---

✅ Step 6: Test the Model (on test data)

# Predict on the test set
y_pred = model.predict(X_test)

# Print test predictions
print("Predicted Labels:", y_pred)
print("Actual Labels   :", y_test.values)

# Evaluate accuracy
from sklearn.metrics import classification_report
print("\nClassification Report:\n", classification_report(y_test, y_pred))


---

✅ Step 7: Predict on New Data

Suppose you have a new flower with features (same order as training data):

# New sample input (same order as X.columns)
new_data = [[5.1, 3.5, 1.4, 0.2]]  # Example: a new Iris sample

# Make prediction
prediction = model.predict(new_data)

# Decode the class name
predicted_class = iris.target_names[prediction[0]]
print("Predicted Class:", predicted_class)


---

🧠 Output Example

Predicted Labels: [1 0 2 ...]
Actual Labels   : [1 0 2 ...]
Classification Report:
              precision    recall  f1-score   support
...
Predicted Class: setosa


---

Would you like this adapted to a regression example or with a different model (like SVM or KNN)?

# Manchendwings-marvels-of-butterfly-species-
