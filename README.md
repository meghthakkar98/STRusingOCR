# Natural Scene Text Recognition (NSTR) Using OCR

## Project Objective

The goal of this project is to build a robust NSTR system that integrates the capabilities of PyTesseract, EasyOCR, and Keras-OCR. Our solution aims to excel in extracting and interpreting text from various natural scene images, overcoming challenges like blurring, distortion, and complex backgrounds. The ultimate ambition is to push the envelope in the field of computer vision, aiding applications such as accessibility tools, data entry automation, and augmented reality interfaces.

## Dataset

Our dataset includes a rich variety of images, combining the ICDAR 2015 dataset known for its complexity, with a selection of in-house captured and annotated visuals. This mix ensures exposure to diverse conditions reflective of real-world text scenarios.

## Methodology

### First Approach

We initiated our project with the EAST text detector to identify text regions, followed by text extraction with PyTesseract. The initial results led us to explore more adaptable OCR solutions.

### Second Approach: Preprocessing Pipeline

1. **Grayscale Conversion**: Simplifying image data to enhance text-background contrast.
2. **Gaussian Blur**: Noise reduction for better thresholding.
3. **Otsu's Thresholding**: Binary transformation to highlight textual elements.
4. **Contour Detection**: Segmentation of textual regions to set the stage for OCR.

### OCR Engines

- **PyTesseract**: Renowned for accuracy and extensive language support.
- **EasyOCR**: Well-suited for real-time applications with noisy backgrounds.
- **Keras-OCR**: Leverages deep learning for end-to-end text detection and recognition.

We visualized the OCR process, drawing bounding boxes to confirm accuracy and compare the performance of the different engines.

## Results

The application of multiple OCR libraries allowed us to assess and utilize their strengths, resulting in a comparison of effectiveness:

- Easy-OCR: Demonstrates proficiency in general text recognition.
- Keras-OCR: Excels in dealing with curved, blurred, and circular text, proving its utility in complex scenarios.

## Conclusion

Keras-OCR provided the best performance in our analyses, proving adept at handling a range of challenging image conditions. However, recognizing text obstructed by elements within images remains a challenge.
