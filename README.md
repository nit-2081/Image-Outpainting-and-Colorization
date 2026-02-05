# Image Outpainting and Colorization Project

This project provides a comprehensive solution for image manipulation with two main capabilities: image outpainting and image colorization. It implements multiple models for colorization, allowing users to choose the best approach for their needs.

## Features

### 1. Image Outpainting
- Extends images beyond their original boundaries
- Provides both raw output and blended results
- Uses a trained GAN model for realistic outpainting

### 2. Image Colorization
Multiple colorization models are implemented:

1. **UNET Scratch Model**
   - Custom implementation of UNET architecture
   - Trained from scratch for colorization

2. **Pretrained UNET Model**
   - Uses a pre-trained UNET model
   - Optimized for better colorization results

3. **DeepLab Model**
   - Implements DeepLab architecture
   - Alternative approach to image colorization

## Web Interface

The project includes a user-friendly Gradio web interface with four tabs:
- Outpainting
- Colorization (UNET Scratch)
- Colorization (Pretrained UNET)
- Colorization (DeepLab)

## Setup and Installation

1. Clone the repository:
```bash
git clone [repository-url]
cd colorization_and_outpainting_5th_sem
```

2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

3. Download the model weights:
   link: https://drive.google.com/drive/folders/1PA_LZyP282gbYl0XrVfkpoDENDyczpcu?usp=sharing
- Outpainting model: `outpaint/G_325.pth`
- UNET Scratch model: `unet_scratch/ImageColorizationModel_8666.pth`
- Pretrained UNET model: `colorization/model_final.pth`
- Pretrained UNET model: `colorization/res18-unet.pth`
- DeepLab model: `deeplab/ImageColorizationModel10.pth`

## Usage

1. Run the application:
```bash
python app.py
```

2. Open the provided URL in your web browser (typically http://localhost:7860)

3. Choose the desired tab for your task:
   - For outpainting: Upload an image to extend its boundaries
   - For colorization: Upload a grayscale image and choose your preferred model

## Model Details

### Outpainting Model
- Uses a GAN-based architecture
- Generates realistic extensions of input images
- Provides both raw and blended outputs for better control

### Colorization Models
1. **UNET Scratch**
   - Custom implementation
   - Good for understanding the colorization process
   - May require more training time

2. **Pretrained UNET**
   - Leverages transfer learning
   - Generally faster and more accurate
   - Better for production use

3. **DeepLab**
   - Specialized in semantic segmentation
   - Can provide more detailed colorization
   - Useful for complex images

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Contributors

- [Shlok Koirala](https://github.com/shlok-py) - Colorization model, Developer
- [Anshu Patel](https://www.linkedin.com/in/anshu-patel-0578a2234/) - Colorization model developer & Model Implementation

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

MIT License

Copyright (c) 2024 Nitesh Rajbanshi

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.



## Acknowledgments

- Gradio for the web interface
- PyTorch for the deep learning framework
- All the model architectures and their original implementations 
