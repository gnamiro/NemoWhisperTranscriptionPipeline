# Diarization and Transcription using NeMo and Whisper
This repo lists the code use to transcribe conversations from case study videos.

The transcription is performed by executing the following steps in a Python pipeline:

## Step 1:
FFmpeg is used to extract the audio out of the case study videos.

## Step 2:
Nvidia's [NeMo](https://github.com/NVIDIA/NeMo) diarization model is used to diarize the audio, which idenifies individual speakers and the audio sections where they are speaking.

## Step 3:
OpenAI's [Whisper](https://github.com/openai/whisper) model is used to transcribe the speaker sections into text.

## Step 4:
The transcribed lines are split and recombined to produce split and merged transcription files for each case study video.

A much more detailed description of the pipeline can be found in the notebooks found in the repo.

## License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.
