# DSC_Final_Project_Group3

The original dataset used was “100random.xlsx,” an Excel spreadsheet containing 100 randomly generated sentences. If you would like to generate different sentences obtained from the same source, visit https://randomwordgenerator.com/sentence.php and transfer the sentences into a spreadsheet. The blocks of code were run in an Amazon Web Services (AWS) Sagemaker ml.t3.medium instance using a JupyterLab notebook running a python_conda3 kernel.

To recreate or adapt our process, connect to this GitHub repo first. In the TextToSpeechMP3 code, the MP3s were stored in an AWS S3 bucket. The first line of that file instructs the reader to create their own S3 bucket in which to store their output files. Where the comments in the code say "insert_name = 'XXXX'", replace the "XXXX" to create a new S3 bucket and store the output data in it. The name must be unique, but so that AWS can properly route files to and from each bucket – AWS will notify you if the name is already taken. Once the bucket is created, run all the code in the file to obtain the Amazon Polly-generated mp3 files.

Second, go into the TranscribedCopy code and change the insert_name = "XXXX" to whatever name you used in the first one. In this code, also make sure to use a unique name for the transcribed work if you are transcribing again (just put a new number in front of the same name if you want). Also, the "levenshtein" package from textdistance was used. 

A more formal walkthrough of the code, reasoning and analysis can be found in the “blog” section.
