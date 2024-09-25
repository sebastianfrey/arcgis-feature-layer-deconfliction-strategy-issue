# arcgis-feature-layer-deconfliction-strategy-issue

Repository contains a reproduction sample to demonstrate an issue with deconfliction strategy on feature layers:

When a filter condition for a feature layer view is delcared and for the label class the deconfliction strategy is set to none, the declared fitler conditionis ignored.

The `index.html` contains a small sampel app, which

1. loads a feature layer
2. declares a labeling info with `deconflictionStrategy=static`
3. sets a filter on the feature layer view
4. renders a radio group, which allows to change the `deconflictionStrategy`

When setting the `deconflictionStrategy` to `none`, only features with `SEASON = 'Winter'` should be shown.
