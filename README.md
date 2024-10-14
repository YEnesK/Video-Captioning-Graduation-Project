# Dense Video Captioning from Human Activity Videos

This project aims to generate detailed captions for human activity videos using both visual and audio features. It utilizes a Bi-modal Transformer model to process and integrate these features, producing accurate and contextually relevant captions for different segments of the video.

## Project Overview

- **Objective**: Create a system that can analyze visual and audio data from videos, identify key events, and generate descriptive captions.
- **Model**: Bi-modal Transformer architecture
- **Dataset**: ActivityNet Captions (subset used for training and evaluation)
- **Features**: Visual (I3D) and Audio (VGGish) features

## Key Components

1. **Feature Extraction**: 
   - Visual features: I3D (Inflated 3D ConvNet)
   - Audio features: VGGish

2. **Bi-modal Transformer**:
   - Encoder: Processes and integrates visual and audio features
   - Decoder: Generates captions based on the processed features
   - Proposal Generator: Identifies important segments in the video

3. **Caption Generation**: Produces detailed captions for identified video segments

## Results

The project compared different configurations:
- Dataset sizes: 2k and 4k videos
- Feature types: Audio-only, Video-only, Audio & Video combined

Evaluation metrics used:
- BLEU_3, BLEU_4
- METEOR
- ROUGE-L
- CIDEr

Key findings:
- Combined audio and video features generally performed best
- Larger dataset size typically improved performance on BLEU and CIDEr metrics
- Some unexpected results observed with METEOR and ROUGE-L metrics

## Future Work

- Expand the dataset size and improve data quality
- Explore additional feature types (e.g., speech recognition)
- Optimize hyperparameters
- Implement user feedback for caption validation and improvement

## Requirements

- Python 3.7+
- PyTorch
- NumPy
- Pandas
- Additional libraries: (list other key libraries)

## Usage

(Include instructions on how to set up the environment, prepare the data, train the model, and generate captions for new videos)

## Contributors

- Yusuf Enes KURT
- Muhammed Ali LALE

## Acknowledgements

This project was completed as part of the Computer Engineering program at Yildiz Technical University, under the supervision of Assoc. Prof. Dr. Ali Can KARACA.


