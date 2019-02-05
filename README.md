# myspokenlanguageid

## Version-5 release with accuracy improvement

### Spoken language identification with CNN and RNN - Early Stage

This program may take a minute or so to get results showed on the screen, please be patient.

Spoken Language Identification is the process of determining and classifying natural language from a given content and dataset. 
Employing an acoustic model and a language model, Data of audio files is processed to extract useful features for performing Machine Learning. 
The acoustic features for SPOKEN LANGUAGE IDENTIFICATION are namely standard features such as Mel-Frequency Cepstral Coefficients (MFCC), 
Shifted Delta Cepstral (SDC), while for the language features the Gaussian Mixture Model (GMM) and the i-vector based framework are used. 

However, the Machine Learning process based on extract features remains a challenge. Optimisation needs to be improved in order to capture embedded knowledge on the extracted features. CNN (Convolutional Neural Networks), RNN (Recurrent Neural Networks) and ELM (the Extreme Learning Machine) are promising as effective learning architectures used to perform classification and further complex analysis and are extremely useful to train a single hidden layer neural network. However, by now, the learning process of these models is not entirely effective due to the selection methods of weights within the input hidden layer.

Myspokenlanguagedetection is a preliminary package structured for SPOKEN LANGUAGE IDENTIFICATION based on standard feature extraction and CNN and RNN. An optimisation approach was employed as the benchmark and improved by altering the selection phase of the optimisation process. The selection process is performed incorporating deferent methods. The results are generated based on SPOKEN LANGUAGE IDENTIFICATION with the datasets created from eighteen different languages. The results of the study indicate the performance of Machine Learning highly correlated with the soundness of architecture of Neural Networks and co-existence of acoustic and language models. 

THIS version of myspokenlanguagedetection was trained to detect 
- "French", 
- "English", 
- "Spanish", 
- "Italian",
- "Deutsch", 
- "Russian", 
- "Portuguese", 
- "Swedish", 
- "Japanese" 

and will increase to more languages as We will progress to complete the machine training sessions for more languages along with increasing the accuracy of the languages identification process.

## Installation

Myspokenlanguagedetection can be installed like any other Python library, using (a recent version of) the Python package 
manager pip, on Linux, macOS, and Windows:

                                        pip install Myspokenlanguagedetection
				
or, to update your installed version to the latest release:

                                     pip install -u Myspokenlanguagedetection 	
                                                    
Recording files must be **25 secs or longer** of audio and in *.wav PCM/LPCM format, recorded at 48 kHz sample frame and 24-32 bits of resolution or AIFF, AIFF-C, FLAC: must be native FLAC format; OGG-FLAC is not supported.

Here is how the myspokenlanguagedetection function behave,  

			[in1]		import my_spoken_language_detection  as mm
				
			[in2]		p=r"C:\Users\my\Desktop\myLanguageIdentification\dataset\audioFiles"
			[in3]		m="audio_file_name" #Set to be in wav format 
			[in4]		mm.myspolangdet(m,p)
				
			[out]		convergence rate %:    29             #the first guess
					convergence rate %:    5
					hold on!! 
					convergence rate %:    40 	      #the second guess
					the language could be: Japanese
					
			[in2] 		mm.myspolangESY()      		      # a quick check function, interactive
			[in2 on shell] 	Enter the path to the Language_Identification directory:
					C:\Users\my\Desktop\myLanguageIdentification\dataset\audioFiles
			[in2 on shell] 	what is your name?    heuiy	      # the audio file name which you wish to analyze 

			[out]	 	convergence rate %:    25
					convergence rate %:    45
					convergence rate %:    7
					convergence rate %:    17
					convergence rate %:    30
					the language could be: English 
			
Please check out EXAMPLES.pdf. 
                                                        
## Development

Myspokenlanguagedetection was developed by MYOLUTIONS Lab in Japan. It is part of New Generation of Voice Recognition and Acoustic & Language modeling Project in MYSOLUTIONS Lab. That is planned to enrich the functionality of Myspokenlanguagedetection by adding more advanced functions. 

