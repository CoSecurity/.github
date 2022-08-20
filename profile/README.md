# CoSecurity
Solution designed to combine security and intelligence in order to make your neighborhood safer.

Our premise is collaborative security through the presence and recording in the cloud, seeking to inhibit criminal actions on the streets of your neighborhood and, if it happens, offering quick action mechanisms to assist in an agile and safe resolution.

We believe that the streets in your neighborhood belong to you and well-meaning people. We don't have to live with fear, but with the certainty of better days. We believe that we should have the right to live safely and share peaceful moments.

## Data Science
We work heavily using computer vision techniques and time series analysis, I have a data ingestion platform allocated on Amazon Web Services (AWS). Among our technologies we can highlight the use of Tensorflow, PyTorch and OpenCV.

Our models are able to perform recognition of people, vehicles and objects in general trained to recognize and determine patterns in the streets of São Paulo. We currently have anomaly detection models for people and vehicles that are able to determine unusual areas and direction taking into account the flow of the road.

All of our models are scaled using AWS SageMaker, interacting via event generations and image loading via AWS S3.

Below is a representation of our architecture from the beginning of image ingestion to the training and prediction stages of the models:
![cosecurity-pipeline drawio-2](https://user-images.githubusercontent.com/29183537/185763035-30ec760b-2a41-444e-a370-e012ba1d8b30.png)

### Project steps
- [x] Project definition
- [x] Cloud definition
- [x] RTSP ingestion
- [x] RTMP ingestion
- [x] Object detection (person, vehicles, etc.)
- [x] Recognition of people's faces on indoor cameras
- [x] Detection of unusual areas on public roads
- [x] Detection of agglomeration of people on public roads
- [x] Detection of oncoming vehicles on public roads
- [ ] Detection of falls on public roads
- [ ] Detection of accident on public roads
- [ ] Detection of clothing types
- [ ] Detection of color
- [ ] Forensic research
- [ ] Sentiment analysis in indoor cameras

