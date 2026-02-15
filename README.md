# Sampling
## Objective
- Balance an imbalanced dataset
- Create five different samples
- Apply five different sampling techniques
- Train five different Machine Learning models
- Determine which sampling technique gives the highest accuracy for each model

## Dataset
- Dataset used: "credit_data.csv"
  
The dataset contains highly imbalanced class distribution:

| Class | Count |
|-------|-------|
| 0     | 763   |
| 1     | 9     |

## Methodology
### Step 1 : Data Balancing (Oversampling)

Since the dataset was highly imbalanced, **SMOTE (Synthetic Minority Oversampling Technique)** was used to balance the classes.

After applying SMOTE:

| Class | Count |
|-------|-------|
| 0     | 763   |
| 1     | 763   |

### step 2 : Creation of Five Samples

Five different samples were created using different random states and fractions:

- Sample1 → 90% of dataset
- Sample2 → 80% of dataset
- Sample3 → 70% of dataset
- Sample4 → 60% of dataset
- Sample5 → 50% of dataset

### step 3 : Sampling Techniques Applied

Five sampling techniques were applied:

1. **Sampling1** → Simple Random Sampling  
2. **Sampling2** → Systematic Sampling  
3. **Sampling3** → Stratified Sampling  
4. **Sampling4** → Cluster Sampling  
5. **Sampling5** → Bootstrap Sampling  

### step 4 : Machine Learning Models Used

Five ML models were trained:

| Model | Name |
|-------|------|
| M1 | Logistic Regression |
| M2 | K-Nearest Neighbors |
| M3 | Decision Tree |
| M4 | Random Forest |
| M5 | Support Vector Machine |

### step 5 : Accuracy Comparison

Each sampling technique was applied to each ML model.

Final output is a 5 × 5 accuracy table:

<img width="372" height="163" alt="image" src="https://github.com/user-attachments/assets/f4cdd1c9-968f-4742-882d-f36c7862b832" />

## Best Sampling Technique

The best sampling technique for each model was determined using:

```
results.idxmax(axis=1)
```

This identifies which sampling method produced the highest accuracy for each ML model.

<img width="96" height="140" alt="image" src="https://github.com/user-attachments/assets/75fd417d-2ea6-4c7f-9735-69658913b161" />

## Conclusion:
- Oversampling significantly improved dataset balance.
- Model performance varies depending on sampling technique.
- Different models respond differently to sampling strategies.
- The best sampling technique depends on the ML model used.
 


