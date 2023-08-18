# Wav2Lip_Lipsync
To attain the desired outcome, we've employed a pre-trained model sourced from Wav2Lip, particularly the Wav2Lip + GAN model. You can access the corresponding GitHub page for this model <a href="https://github.com/Rudrabha/Wav2Lip">here</a>.
- Link for the input audio and video used:  https://drive.google.com/drive/folders/1U8-gKy0GQXUFWM0MdDbM_G61BhnjNdqn
## Resultant video:
https://github.com/FozanAzhar/AI_LipSync_Wav2lip/assets/95569589/bb7f26b4-fd95-4308-b803-cde044764000




## Steps

Step 1: Setup Wav2Lip

Install dependencies
Download the pretrained Wav2Lip model from a URL and save it to the appropriate directory.
Clone the Wav2Lip repository from GitHub.
Download a pretrained model for face detection and save it to the appropriate directory.
Install the required Python packages.

Step 2: LipSync for downloading a YouTube video

Install yt-dlp to download YouTube videos.
Provide a YouTube URL.
Trim the video based on specified start and end times.

Step 3: Select Audio (Record, Upload from local drive, or Gdrive)

Choose the method to provide audio input (Record, Upload, or Custom Path).
If 'Record' is selected, record audio.
If 'Upload' is selected, upload an audio file.
If 'Custom Path' is selected, provide the full path to the audio file on Google Drive.

Step 4: Start Crunching and Preview Output

Specify padding values for the input video frames.
Specify the rescale factor for the video frames.
Choose whether to enable or disable smoothing.
Use the Wav2Lip model to generate lip-synced output.
Display the final lip-synced video and provide a download link for it.

Note: The provided code uses Google Colab specific commands for file uploading and audio recording, which may not work outside the Colab environment without adjustments.
