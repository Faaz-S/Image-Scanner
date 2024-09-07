# Image Scanner

Necessary libraries:

- boto3 for interacting with AWS services.
- matplotlib for visualization.
- PIL (Python Imaging Library) for handling image data.
- BytesIO from the io module to work with image data.

## detect_labels function

This function takes a photo and bucket name as input parameters. Within the function:

1. We create a Rekognition client using boto3.
2. We use the detect_labels method of the Rekognition client to detect labels in the given photo.
3. We print the detected labels along with their confidence levels.
4. We load the image from the S3 bucket using boto3 and PIL.
5. We use matplotlib to display the image and draw bounding boxes around the detected objects.

# main function

A main function to test our detect_labels function. We specify a sample photo and bucket name, then call the detect_labels function with these parameters.

# USE INSTRUCTIONS

1. Fork the repo
2. Install required libraries
3. Create an IAM user in your AWS console and configure your CLI with IAM access keys.
4. Create an S3 bucket and upload the images you want to scan
5. Replace the your-bucket-name and your-image-name with the names of your bucket and image path.
6. Run the python file in the command line
