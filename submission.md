### Links to W&B and Github
* W&B:
* Github repository:

Watch out! best model has been selected by setting parameters `modeling.max_tfidf_features` to 10, 15 and 30, and `modeling.random_forest.max_features` to 0.1, 0.33, 0.5, 0.75, 1.

Best parameters:
* `modeling.max_tfidf_features` = 15
* `modeling.random_forest.max_features` = 0.5

### Final test

```shell
> mlflow run . -P steps=all
```

WATCH OUT! Run `divine-night-31` (type=`train_random_forest`) has been generated with the above command and, as expected, it provides the same results as run `denim-surf-18`, which corresponds to production model. It seems that W&B does not lineage both models.


### 

```shell
> mlflow run https://github.com/irenerodriguez/nd0821-c2-build-model-workflow-starter.git \
  -v 1.0.0 \
  -P hydra_options="etl.sample='sample2.csv'"
```