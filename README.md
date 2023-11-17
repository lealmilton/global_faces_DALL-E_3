# 🌍 Global Faces: A DALL-E 3 Project 🌐

This project utilizes OpenAI's DALL-E to generate images representing people from every country recognized by the United Nations. The goal is to create a unique visual representation for each country, encapsulating its diverse identities.

Note: Sudan and South Sudan had to be excluded from the list because of OpenAI's API restrictions.

## 🚀 Getting Started
Here's how to set up and run the Global Faces project:

Install necessary libraries:

```
!pip install imageio-ffmpeg openai requests
```

Run the Python notebook provided. This script includes a list of all UN-recognized countries and the code necessary to generate and download images.

The script includes functions to check if an image for a country already exists and to generate and save images with rate limiting to avoid API overload.

Execute the main function to generate images for all UN countries. It will skip countries for which images already exist and apply rate limiting to manage API usage.

## 🔧 Script Overview

- Country List: A comprehensive list of all countries recognized by the United Nations.
- OpenAI Client Initialization: Sets up the client for API requests.
- Image Generation: A function to generate an image for each country using DALL-E, with the country's name included in the image.
- Rate Limiting: To manage API calls and adhere to OpenAI's usage guidelines.
- Image Download and Save: Functionality to download and store the images locally.
- Video Creation: After generating images, a video is compiled showcasing all the images, providing a visual journey across the globe.

## 📂 Project Structure

- people/: Directory where generated images are stored.
- people.ipynb: The primary Python notebook that runs the image generation and video creation process.
- countries_video.mp4: The output video file showcasing images from all countries.

## 🎯 Project Output

- Generated Images: Images representing people from each country, stored in the people directory.
- Video Showcase: A compiled video of all generated images, providing a visual representation of global diversity.

## 📌 Note
Make sure to have your OpenAI API key set up correctly in a .env file for accessing DALL-E, as the script requires this for image generation.
