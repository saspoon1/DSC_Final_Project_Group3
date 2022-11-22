# DSC_Final_Project_Group3

The original dataset used was “100random.xlsx” It was 100 randomly generated sentences. If you want to use your own sentences you can make an excel file and change them. 

The blocks of code were run in an AWS Sagemaker ml.t3.medium instance, using a jupyterlab notebook running python_conda3. Connect to this GitHub repo first. In the TextToSpeachMP3 code, the MP3s were stored in an AWS S3 bucket. In the first line it says insert_name = "XXXX", you can replace the "XXXX" (or whataver is there) with whataver you want as long as it's unique (just remeber it for later) to store it in your own s3 bucket. Then run all the code.

Second, go into the TranscribedCopy code and change the insert_name = "XXXX" to whataver name you used in the first one. In this code, also make sure to use a unique name for the transcribed work if you are transcribing again (just put a new number in front of the same name if you want). Also, the "levenshtein" package from textdistance was used. 

A more formal walkthrough of the code, reasoning and analysis can be found in the “blog” section.
