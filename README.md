
# Automatic Hindu Mythology Shorts Creator

This Python script automatically generates short videos based on random Hindu mythology stories. It:

- Fetches a random story from the LLaMA API
- Generates Raja Ravi Varma-style images using Stable Diffusion
- Converts story narration to speech using Edge TTS
- Creates animated text overlays with large, centered words
- Compiles everything into a seamless short video

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/shorts-creator.git
   cd shorts-creator
   ```

2. Install dependencies:
   ```sh
   pip install torch diffusers moviepy edge-tts requests huggingface_hub numpy pillow nest_asyncio
   ```

3. Set up API keys:
   - Replace `"your_llama_api_key_here"` in `script.py` with your LLaMA API key
   - Replace `"hf_abcd"` in `main.py` with your Hugging Face token

## Usage

Run the script:
```sh
python script.py
```

### Output
- `final_video.mp4` (the generated short video)
- Images saved in `generated_images/`
- Audio files stored in `generated_audio/`

## Customization

- **Text Size & Position**: Modify `font_size` in `create_word_by_word_clips()` inside `script.py` to adjust text size
- **Image Quality**: Change `guidance_scale` in `generate_image_with_stable_diffusion()` for better image refinement
- **Story Duration**: Adjust `clip_duration` for each segment inside `fetch_random_story()`

## Features

- ✅ **Fully Automated** – No manual input required
- ✅ **HD Video Output** – Generates 1080p videos with professional-quality images
- ✅ **Traditional Art Style** – Uses Raja Ravi Varma-style painting effects
- ✅ **Smooth Transitions** – Includes fade-in/out effects for seamless storytelling
- ✅ **Optimized for Shorts** – Generates engaging, word-by-word animated text

## License

This project is open-source under the MIT License.
