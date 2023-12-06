# Solar-Irradiance-Prediction
We aim to predict solar irradiance using meterological data and all sky images from 2021-2023 by exploring various modeling techniques.

### Modeling Meteorological Data
We explored multiple models such as ARIMA, Prophet, LSTM to forecast solar irradiance. Prophet demonstrated the best results of these techniques.

### Modeling All-sky Images
The first step for modeling an image regression model was to perform segmentation of the all-sky images; we used BRBG alorithm to do this.

Following this, various pre-trained models such as Inception, Mobilenet and vgg16 were explored. We also trained a custom CNN image regression model.

## Hybrid Modeling
This architecture is an ensemble of the best model from the meteorological model and image regression model. Using the predictions from both these models, one single soalr irradiance forecast is provided.

## Multimodal Modeling
This architecture combines both the meteorological and image features. A single forecasting model is trained using all the combined features.
