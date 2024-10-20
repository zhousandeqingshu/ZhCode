#  Corresponding paper:
InSeC: Steganalysis Model Based on Inter-codeword Sensitivity Caption for Compressed Speech Streams

# Research content:
Recently, steganalysis of VoIP compressed speech has gained attention. In real voice communication, Joint Parallel Steganography (JPS) often occurs, where multiple steganography algorithms coexist. The multifaceted nature of JPS, incorporating various steganographic algorithms, poses significant challenges in steganalysis. We believe that detecting JPS accurately requires multi-stage feature extraction, as a single-stage approach fails to yield satisfactory results. In this paper, we propose an efficient steganalysis model based on Inter-codeword Sensitivity Caption, termed InSeC. It consists of two neural modules: the steganography-sensitive codeword-pair caption module, which analyzes changes in codeword pairs before and after modification from multiple perspectives and aggregates these features, and the fine-grained correlation re-perception module, which re-evaluates features within a local range. Our method achieved a
25.27%, 11.57%, and 9.07% improvement in detection accuracy compared to three recent RNN- and CNNbased methods on the JPS detection task with a 20% embedding rate in the English dataset.


# Instructions:
1. Download the code. zip file and follow the guide. txt file to perform the corresponding operations.
2. This model code needs to change the corresponding parameters in the ablation experiment, and users can conduct the 
   experiment themselves according to the prompts in the code.
3. The run.py contains functions written for training, testing, validation, time consumption, and more.
