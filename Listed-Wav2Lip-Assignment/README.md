# Listed_Wav2Lip_Lipsync

The model can be implemented by executing the cells one by one in the notebook Listed_Wav2Lip.ipynb.

Drive Link:  https://drive.google.com/drive/folders/1U8-gKy0GQXUFWM0MdDbM_G61BhnjNdqn

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
