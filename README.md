
# Furniture Classification Project

The goal of this project is to improve an image classification model to identify furniture from an input image. The current model can categorize furniture and provide additional details like the supplier's name and purchase URL.

## Purpose
### Long-term Objective

We aim to develop a multimodal model capable of processing inputs such as images, text, and even audio to identify furniture names, categories, and images.

### Future Features:

- **Text Input**: Allow users to provide an approximate description of furniture (supplier, brand, color, etc.) and receive one or multiple suggestions with probability scores for each item.
- **Image Input**: Enable users to take one or more photos (e.g., with a phone) and receive the furniture category, name, supplier, and, if available, a purchase URL.

## Resources
- Model Repository
- Datasets

## Quick Start

For those who prefer not to train the model themselves, a pre-trained model is available on Hugging Face. You can download it here.

### Download the Model

After downloading, place the `furniture_classifier_model.h5` file in the `model` folder.

### Start Training

```bash
cd model
python train_model.py
```

### Launch the Project with Docker

1. Build the Docker image:

   ```bash
   docker-compose build
   ```

2. Start the container:

   ```bash
   docker-compose up
   ```

The API will be available at [http://localhost:80](http://localhost:80). You can access the web interface or use the API endpoints to predict and train the model.