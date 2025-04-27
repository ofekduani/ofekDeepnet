# DeepFilterNet Audio Processing Project

This repository contains audio processing and enhancement tools based on DeepFilterNet.

## How to Clone and Run This Project

### Step 1: Clone the Repository
```bash
git clone https://github.com/ofekduani/ofekDeepnet.git
cd ofekDeepnet
```

### Step 2: Clone DeepFilterNet
```bash
git clone https://github.com/Rikorose/DeepFilterNet.git
```

### Step 3: Install Dependencies
```bash
cd DeepFilterNet
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
pip install -e .
```

### Step 4: Run the Pipeline
To process an audio or video file:
```bash
cd DeepFilterNet
./flexaudio_pipeline.sh -i /path/to/your/audio_or_video_file.mp4 -config configs/denoise_only_pipeline.yaml
```

### Available Pipeline Configurations
- `configs/denoise_only_pipeline.yaml` - Basic noise reduction
- `configs/diarization_pipeline.yaml` - For speaker diarization
- `configs/denoise_speed_pipeline.yaml` - Noise reduction with speed adjustment
- `configs/diarization_enhanced_pipeline.yaml` - Enhanced diarization

## Output
The processed audio file will be saved in the DeepFilterNet directory with the name format: `[input_filename]_ready.wav` 