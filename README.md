# Real Estate Progression - House Detection

## Overview
This project focuses on detecting and counting the number of houses in an image using an object detection model. A custom dataset was created, and the model was trained using RoboFlow and Ultralytics YOLO.

## Project Workflow
1. **Dataset Creation:**
   - Collected images of households.
   - Labeled buildings manually using RoboFlow to create an object detection model.
   
2. **Model Training:**
   - Used RoboFlow to annotate images and train the model for house detection.
   - Fine-tuned the model to improve accuracy.

3. **Implementation in Google Colab:**
   - Installed Ultralytics and RoboFlow in Google Colab.
   - Provided the API key to access the trained model.

4. **Image Processing:**
   - Wrote a script that takes an image from the dataset (e.g., `001.jpg`).
   - The model detects the number of houses in the image.
   - Generates an output image with a new filename format: `{original_filename}_Houses_{house_count}.jpg` (e.g., `V001_Houses_0.jpg` for an image where 0 houses were detected).

## Example
| Input Image | Detected Houses | Output Filename |
|------------|----------------|----------------|
| `001.jpg` | 0 | `001_Houses_0.jpg` |
| `002.jpg` | 3 | `002_Houses_3.jpg` |

## Requirements
- Python
- Google Colab
- RoboFlow API Key
- Ultralytics YOLO

## Installation & Usage
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/real-estate-progression.git
   cd real-estate-progression
   ```
2. Install dependencies in Google Colab:
   ```python
   !pip install ultralytics roboflow
   ```
3. Authenticate with RoboFlow API:
   ```python
   from roboflow import Roboflow
   rf = Roboflow(api_key="YOUR_API_KEY")
   ```
4. Run the detection script and process images.

## Future Enhancements
- Improve model accuracy with more training data.
- Implement a web-based interface for easy image uploads.
- Integrate GIS data for better real estate insights.

## Contributing
Feel free to submit issues or pull requests to enhance the project!

## License
This project is licensed under the MIT License.

---
### Let's build smarter real estate solutions with AI! 🏠🚀

