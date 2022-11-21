# DSC_Final_Project_Group3


The original dataset used was “100random.xlsx” It was 100 randomly generated sentences. If you want to use your own sentences you can make an excel file and change them. 

The blocks of code were run in an AWS Sagemaker ml.t3.medium instance, using a jupyterlab notebook running python_conda3. Run the textToSpeach code first, the transcription code second, and the analysis code third. 

In the first chunk, the MP3s were stored in an AWS S3 bucket. You can change it around to store it in a new location, but be sure to adjust the path in the second chunk as well. Also, be sure that permissions in that bucket are set to be public so the second code chunk can access it without error. Finally, make sure to use a unique name for the transcribed work if you are transcribing again (just put a new number in front of the same name). 

In the analysis section, the python "levenshtein" package from textdistance was used. 

A more formal walkthrough of the code, reasoning and analysis can be found in the “blog” section.
