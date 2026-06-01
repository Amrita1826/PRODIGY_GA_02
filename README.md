# DALL-E Mini Image Generator 🎨

## Overview

This project demonstrates the use of **DALL-E Mini (MinDalle)** to generate AI-powered images from text prompts. The notebook loads a pre-trained DALL-E Mini model, generates multiple image variations based on a user-defined prompt, and displays the results in a grid format.

## Features

- Generate images from natural language descriptions
- Uses the MinDalle implementation of DALL-E Mini
- Supports GPU acceleration with CUDA
- Creates multiple image variations for a given prompt
- Displays generated images in a grid
- Allows selection and saving of the best image

## Technologies Used

- Python
- PyTorch
- MinDalle
- NumPy
- Matplotlib
- Pillow (PIL)
- OpenAI CLIP

## Installation

Install the required dependencies:

```bash
pip install min-dalle
pip install torch torchvision
pip install ftfy regex tqdm
pip install git+https://github.com/openai/CLIP.git
pip install pillow matplotlib numpy
```

## Usage

### 1. Define the Text Prompt

```python
TEXT_PROMPT = "a place with beautiful scenery, digital art"
```

### 2. Configure Generation Parameters

```python
NUM_IMAGES = 9
GRID_SIZE = 3
SEED = 42
SUPERCONDITION_FACTOR = 16
TOP_K = 256
```

### 3. Generate Images

```python
image = model.generate_image(
    text=TEXT_PROMPT,
    seed=SEED,
    grid_size=GRID_SIZE,
    temperature=1,
    top_k=TOP_K,
    supercondition_factor=SUPERCONDITION_FACTOR
)
```

### 4. View Results

The notebook generates a grid of AI-created images based on the provided prompt. Users can select the best image from the generated outputs.

## Project Structure

```text
├── DALL_E_Mini_Image_Generator_internship_Copy.ipynb
├── README.md
```

## Example Prompt

```text
a place with beautiful scenery, digital art
```

## Future Enhancements

- Web interface using Streamlit or Gradio
- Higher-resolution image generation
- Multiple artistic styles
- Automatic image download functionality
- Prompt history management

## Learning Outcomes

- Understanding text-to-image generation
- Working with pre-trained generative AI models
- Image processing using Python
- GPU-based deep learning inference
- Using DALL-E Mini for creative AI applications

## Author

**Amrita Khosla**

## License

This project is developed for educational and learning purposes.
