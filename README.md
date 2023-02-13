# PyData NYC Timeseries Forecasting Tutorial

This repo contains the material for my PyData NYC tutorial on Large Scale Timeseries Forecasting.

In this tutorial, we use the [M5 Forecasting Accuracy](https://www.kaggle.com/competitions/m5-forecasting-accuracy) competition data. This contains Walmart sales data for the USA for over 3000 products. We will use distributed computing to run multiple models for each timeseries and get the best forecasts.

We will use Nixtla's lightning fast [statsforecast] library to run statistical and econometric models at scale. In order to preprocess data, we will use [Fugue](https://github.com/fugue-project/fugue/) to define logic in Python or Pandas, and then port it to Spark, Dask, or Ray. The combination of these two tools will allow us to develop models on large datasets. Because Fugue is agnostic to any framework, the approach illustrated here will work for Spark, Dask, and Ray with minimal tweaks.

The fourth section of the tutorial focuses on Hierarchical Forecasting, where we want to make sure that the forecasts at different levels (store/region/state) are consistent with each other when we add them up.

The last part will be about distributing the model training on a Dask cluster managed by [Coiled](https://www.coiled.io/). Included are best practices around passing data to workers.

## Contact Us

If you want me to give this tutorial, just feel free to reach out! It took a lot of work to compile this tutorial so I'm more than happy to speak about it anywhere (even in company knowledge sharing sessions).

[Fugue Slack](slack.fugue.ai)

[Nixtla Slack](https://join.slack.com/t/nixtlaworkspace/shared_invite/zt-135dssye9-fWTzMpv2WBthq8NK0Yvu6A)

My email:
kdykho@gmail.com

