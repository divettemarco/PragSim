# A Corpus of Pragmatic-Similarity Judgments over Spoken-Dialog Utterances
This is a collection of 1,980 pragmatic-similarity judgments of spoken-dialog utterance pairs. 
## Expected Uses

## Collection Procedure

## Directory Structure and File Formats
judgments/judgment-data.xlsx is the main data set for 220 stimuli total. Each row has columns for the stimuli #, stimuli name, seed name, and reenactment pair name as well as the judgments given by the 9 participants.

The stimuli used in the judgment session are found in stimuli-reordered, with 458 total, and kids-stimuli, with 5 total, which is an overall total of 463 stimuli. The seed utterances chosen for creating the stimuli are found in seeds while the reenactments of those utterances are found in reenactments. The full dialogue-conversations from which the seeds were retrieved from are found in full-conversations which also has files of the reenactments created by the reenactors. All audio is in 16KHz format. The stimuli, seeds, reenactments, and reenactment files are all one channel. All other audios are 2 channel.

metadata/judge-data.xlsx contains the ID, gender, and age of all 9 participants. metadata/source-conversations.xlsx contains information on each speaker found from the seeds including their ID and source conversation, the names of the source recordings, track, corpus name, and the URL for the corpus from which the source conversations were found. metadata/reference-conversations.xlsx contains information on the reenactors including an ID, the names of their full reenactment recordings, gender, age, and name.
