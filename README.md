# LipSync with Wav2Lip

This project is an implementation of a LipSync tool using the Wav2Lip framework. It allows you to synchronize audio and video streams in real-time, creating a seamless and natural lip movement effect. The tool utilizes the Wav2Lip + GAN pre-trained model to achieve this synchronization.

Drive link (Output) : https://drive.google.com/drive/folders/1U8-gKy0GQXUFWM0MdDbM_G61BhnjNdqn?usp=drive_link

## Setup

To set up the project, follow these steps:

1. Install Dependencies: The required dependencies can be installed by running the provided code. This includes the necessary packages for audio processing, video editing, and model inference.

   `!rm -rf /content/sample_data`
   `!mkdir /content/sample_data`

- Clone the repository:

   ```bash
   !git clone https://github.com/FozanAzhar/AI-Lipsync
   ```

2. Download Pretrained Model: The Wav2Lip + GAN pretrained model is automatically downloaded using the provided code. This model is the backbone of the LipSync tool and ensures accurate synchronization between audio and video.

     ``` bash
     !wget 'https://iiitaphyd-my.sharepoint.com/personal/radrabha_m_research_iiit_ac_in/_layouts/15/download.aspx?share=EdjI7bZlgApMqsVoEUUXpLsBxqXbn5z8VTmoxp55YNDcIA' -O 
     '/content/Wav2Lip/checkpoints/wav2lip_gan.pth'
      ```

- Install FFmpeg Python package:

   ``` !pip install ffmpeg-python ```

3. Face Detection Model: A pretrained face detection model is also included in the setup. This model helps in accurately detecting faces in videos.

  ```bash
  !wget "https://www.adrianbulat.com/downloads/python-fan/s3fd-619a316812.pth" -O "/content/Wav2Lip/face_detection/detection/sfd/s3fd.pth"
  ```

4. Audio Recording: The project provides functionality to record audio directly in the Colab environment. This is done through audio recording code that utilizes the browser's capabilities.

## Usage

1. LipSync with YouTube Video: You can easily LipSync any YouTube video by providing its URL. The tool allows you to trim the video to the desired start and end times before performing the synchronization.

2. Uploading Custom Video: If you have your own video, you can upload it for LipSyncing. The tool even provides an option to resize higher resolution videos to 720p to ensure compatibility.

3. Audio Input Options: You can choose to record audio directly within the Colab environment or upload your own audio file. The tool supports various audio formats.

4. Advanced Settings: The project allows you to customize certain parameters for the LipSyncing process, including padding, resizing, and smoothing options.

## How It Works

The project combines audio and video streams using the Wav2Lip + GAN model. The code handles the LipSyncing process by accurately mapping the audio's phonetic content to the corresponding lip movements in the video. This creates a convincing LipSync effect that enhances the naturalness of the video.

## Limitations

1. Video Length: The tool is designed for videos up to 60 seconds in length. Longer videos may not produce accurate results.

2. Face Presence: The quality of the LipSync effect depends on having a face present in all frames of the video.

## Final Output

After processing, the tool generates a LipSynced video where the lip movements are synchronized with the audio. The output video is available for preview and download.

## Resultant preview 

https://github.com/FozanAzhar/AI_LipSync_Wav2lip/assets/95569589/08164e6c-8d8d-4e38-9182-173bbb64c617

## Acknowledgments
This project is built upon the Wav2Lip framework developed by [prajwalkr](https://github.com/Rudrabha/Wav2Lip).
