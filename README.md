# 7th place - post competition
Hello everyone,

I have built a model with which I have obtained an AUC = 0.828314 for the private classification.

This model is an ensemble of ensembles of various XGBOOST models.

Best XGBOOST Models:

1) TomekLink + ENN + XGB (max_depth = 5, n_rounds = 500, eta = 0.020204812)

2) TomekLink + ENN + XGB (max_depth = 5, n_rounds = 500, eta = 0.0202048125)

3) ENN + XGB (max_depth = 5, n_rounds = 500, eta = 0.020204813)

4) ENN + TomekLink + XGB (max_depth = 4, n_rounds = 560, eta = 0.020204812)

5) undersampling (30) + XGB (max_depth = 5, n_rounds = 300, eta = 0.020204812)

6) TomekLink + ENN + Delim. Characteristics +XGB(max_depth=5, n_rounds=600, eta=0.020204812)

7) undersampling (30) + XGB (max_depth = 5, n_rounds = 300, eta = 0.0202048123)

Ensemble: Arithmetic mean of the predictions of each XGBOOST model.

E1) (1 + 2 + 3 + 4 + 5 + 6 + 7) / 7

E2) (1 + 3 + 4) / 3

Final Ensemble: (E1 + E2) / 2