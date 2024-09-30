## Project Overview

This project, "Baking with Gemini API," is a work in progress and a strong candidate for my capstone project. It demonstrates the integration of Google's Gemini API with image recognition capabilities to generate recipes based on images of baked goods.

**Note: This project is currently under development and may undergo significant changes.**

## Prerequisites

Before you begin, ensure you have the following installed:
- Python 3.7 or higher
- pip (Python package installer)

## Setup

1. Clone this repository to your local machine.

2. Install the required dependencies:
   ```
   pip install langchain langchain-google-genai Pillow ipython
   ```

3. Obtain a Google API key:
   - Visit the [Google AI Studio](https://makersuite.google.com/app/apikey)
   - Create a new API key
   - Copy the API key

4. Set up your Google API key:
   - Open the script and replace `<YOUR_API_KEY>` with your actual Google API key:
     ```python
     os.environ['GOOGLE_API_KEY'] = '<YOUR_API_KEY>'
     ```

## Usage

1. Prepare an image of baked goods you want to generate a recipe for.

2. Update the image path in the script:
   ```python
   img = PIL.Image.open('path_to_your_image.jpg')
   ```

3. Customize the prompt if desired:
   ```python
   prompt = 'Provide an example recipe for the baked goods in the image'
   ```

4. Run the script. It will:
   - Load the specified image
   - Send the image and prompt to the Gemini API
   - Stream and display the generated recipe

## Project Structure

- `main.py`: The main script containing the code to interact with the Gemini API
- `baked_goods_1.jpg`, `baked_goods_2.jpg`, `baked_goods_3.jpg`: Sample images for testing (you can add your own)

## Future Improvements

As this project is a work in progress, there are several areas for potential improvement:

1. Implement error handling and input validation
2. Create a user-friendly interface (web or desktop application)
3. Add functionality to save and categorize generated recipes
4. Implement a feature to compare multiple recipes or suggest modifications
5. Integrate with a database to store and retrieve past results

## Contributions

As this is a capstone project candidate, contributions are currently not being accepted. However, feedback and suggestions are welcome and can be submitted as issues in the project repository.

## License


## Disclaimer

This project is for educational purposes only. Ensure you comply with Google's Gemini API terms of service and usage policies.