# myspokenlanguageid
Spoken language identification with CNN and RNN - Early Stage

Spoken Language Identification is the process of determining and classifying natural language from a given content and dataset. 
Employing an acoustic model and a language model, Data of audio files is processed to extract useful features for performing Machine Learning. 
The acoustic features for SPOKEN LANGUAGE IDENTIFICATION are namely standard features such as Mel-Frequency Cepstral Coefficients (MFCC), 
Shifted Delta Cepstral (SDC), while for the language features the Gaussian Mixture Model (GMM) and the i-vector based framework are used. 

However, the Machine Learning process based on extract features remains a challenge. Optimisation needs to be improved in order to capture embedded knowledge on the extracted features. CNN (Convolutional Neural Networks), RNN (Recurrent Neural Networks) and ELM (the Extreme Learning Machine) are promising as effective learning architectures used to perform classification and further complex analysis and are extremely useful to train a single hidden layer neural network. However, by now, the learning process of these models is not entirely effective due to the selection methods of weights within the input hidden layer.

Myspokenlanguagedetection is a preliminary package structured for SPOKEN LANGUAGE IDENTIFICATION based on standard feature extraction and CNN and RNN. An optimisation approach was employed as the benchmark and improved by altering the selection phase of the optimisation process. The selection process is performed incorporating deferent methods. The results are generated based on SPOKEN LANGUAGE IDENTIFICATION with the datasets created from eighteen different languages. The results of the study indicate the performance of Machine Learning highly correlated with the soundness of architecture of Neural Networks and co-existence of acoustic and language models. 

THIS version of myspokenlanguagedetection was trained to detect "French", "English", "Spanih", "Italian", "Deutsch", "Russian", "Portuguese", "Swedish", and "Japanese" and to some lower extent other 40 languages. We will complete the machine training 
sessions for morelanguages along with increaing the accuracy of the languages identification process.

                                                          Installation
                                                         =============
Myspokenlanguagedetection can be installed like any other Python library, using (a recent version of) the Python package 
manager pip, on Linux, macOS, and Windows:

                                                    pip install mypokenlanguage
				
or, to update your installed version to the latest release:
                                                    pip install -u mypokenlanguage 	
                                                    
Recording files must be 15 secs or less of audio and in *.wav PCM/LPCM format, recorded at 48 kHz sample frame and 24-32 bits of resolution or AIFF, AIFF-C, FLAC: must be native FLAC format; OGG-FLAC is not supported.

Here is how the myspokenlanguagedetection function behave,  
						[in1]		import myspokenlanguagedetection as mysp
						[in2]		p=r"C:\Users\name\Desktop\directory_for_audio_files" 
						[in3]		m="audio_file_name" #Set to be in wav format 
						[in4]		mysp.myspolangdet(m,p)
						
						[out]		probability degree: [fr:99.95%]             #the first guess
								the language could be: French
								probability degree: [sv:85.72%, it:14.28%]  #the second guess
								the language could be: Swedish
  
Myspokenlanguagedetection was developed by MYOLUTIONS Lab in Japan. It is part of New Generation of Voice Recognition and Acoustic & Language modelling Project in MYSOLUTIONS Lab. That is planned to enrich the functionality of Myspokenlanguage by adding more advanced functions.

                                                        Development

Myspokenlanguagedetection was developed by MYOLUTIONS Lab in Japan. It is part of New Generation of Voice Recognition and Acoustic & Language modelling Project in MYSOLUTIONS Lab. That is planned to enrich the functionality of Myspokenlanguagedetection by adding more advanced functions. 

