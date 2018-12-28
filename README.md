# myspokenlanguageid
Spoken language identification with CNN and RNN - Early Stage

Spoken Language Identification is the process of determining and classifying natural language from a given content and dataset. 
Employing an acoustic model and a language model, Data of audio files is processed to extract useful features for performing Machine Learning. 
The acoustic features for SPOKEN LANGUAGE IDENTIFICATION are namely standard features such as Mel-Frequency Cepstral Coefficients (MFCC), 
Shifted Delta Cepstral (SDC), while for the language features the Gaussian Mixture Model (GMM) and the i-vector based framework are used. 

However, the Machine Learning process based on extract features remains a challenge. Optimisation needs to be improved in order to capture embedded knowledge on the extracted features. CNN (Convolutional Neural Networks), RNN (Recurrent Neural Networks) and ELM (the Extreme Learning Machine) are promising as effective learning architectures used to perform classification and further complex analysis and are extremely useful to train a single hidden layer neural network. However, by now, the learning process of these models is not entirely effective due to the selection methods of weights within the input hidden layer.

Myspokenlanguage is a preliminary package structured for SPOKEN LANGUAGE IDENTIFICATION based on standard feature extraction and CNN and RNN. An optimisation approach was employed as the benchmark and improved by altering the selection phase of the optimisation process. The selection process is performed incorporating deferent methods. The results are generated based on SPOKEN LANGUAGE IDENTIFICATION with the datasets created from eighteen different languages. The results of the study indicate the performance of Machine Learning highly correlated with the soundness of architecture of Neural Networks and co-existence of acoustic and language models.   

                                                          Installation
                                                         =============
Mypokenlanguage can be installed like any other Python library, using (a recent version of) the Python package 
manager pip, on Linux, macOS, and Windows:

                                                    pip install mypokenlanguage
				
or, to update your installed version to the latest release:
                                                    pip install -u mypokenlanguage 	
                                                    
Recording files must be 15 secs or less of audio and in *.wav PCM/LPCM format, recorded at 48 kHz sample frame and 24-32 bits of resolution or AIFF, AIFF-C, FLAC: must be native FLAC format; OGG-FLAC is not supported.

Here is how the myspokenlanguage function behave,  
						[in1]		import myspokenlanguage as mysp
						[in2]		p=r"C:\Users\name\Desktop\directory_for_audio_files" 
						[in3]		m="audio_file_name" #Set to be in wav format 
						[in4]		y=mysp(m,p)
						
						[out]		The audio file is detected
								**********************************************
								Langauges codes, please refer toList of ISO 639-1 codes
								[['ca', 'Catalan'], ['cy', 'Welsh'], ['da', 'Danish'], ['de', 'Deutsch'], ['en', 'English'], ['es', 'Spanish'], 
								['et', 'Estonian'], ['fi', 'Finnish'], ['fr', 'French'], ['hr', 'Croatian'], ['hu', 'Hungarian'], ['it', 'Italian'], 
								['lt', 'Lithuanian'], ['lv', 'Latvian'], ['nl', 'Dutch'], ['no', 'Norwegian'], ['pl', 'Polish'], ['pt', 'Portuguese'], 
								['ro', 'Romanian'], ['ru', 'Russian'], ['sk', 'Slovak'], ['sl', 'Slovene'], ['sv', 'Swedish'], 
								['tl', 'Tagalog'], ['tr', 'Turkish']]
								**********************************************
								probability degree: [English:0.95]
								the language could be: English
  
Myspokenlanguage was developed by MYOLUTIONS Lab in Japan. It is part of New Generation of Voice Recognition and Acoustic & Language modelling Project in MYSOLUTIONS Lab. That is planned to enrich the functionality of Myspokenlanguage by adding more advanced functions.

                                                        Development

Myspokenlangguage was developed by MYOLUTIONS Lab in Japan. It is part of New Generation of Voice Recognition and Acoustic & Language modelling Project in MYSOLUTIONS Lab. That is planned to enrich the functionality of Myspokenlanguage by adding more advanced functions. 

