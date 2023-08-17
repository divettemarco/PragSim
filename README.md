# A Corpus of Pragmatic-Similarity Judgments over Spoken-Dialog Utterances
This is a collection of 1,980 pragmatic-similarity judgments of spoken-dialog utterance pairs. Judgments are done on a continuous scale of 0 to 4, where 0 represents no similarities between an utterance pair and 4 represents almost identical. Each pair consists of a seed, taken from a real dialog and a reenactment, separated by a beep. The reenactments were created using 6 methods described in a conference paper under preparation.

## Expected Uses
This data is intended to be used or training an automatic model of similarity.

## Collection Procedure
Judgments were collected in a four hour judgment session where there were 9, mostly naive, judges in one room. They were trained and then listened to the stimuli and gave judgments. Judgments were entered using a QuestionPro form: https://utepsubacc.questionpro.com/t/AX8ttZzJBn.

## Directory Structure and File Formats
judgments/judgment-data.xlsx is the main data set for the 220 stimuli judged so far. Each row has columns for the stimulus #, stimulus name, seed name, and reenactment name as well as the judgments given by the 9 participants.

The stimuli used in the judgment session are found in stimuli-reordered/, with 458 total, and kids-stimuli/, with 5 total, which is an overall total of 463 stimuli. We only used the first 220 stimuli in the judgment session. The seed utterances chosen for creating the stimuli are found in seeds/ while the reenactments of those utterances are found in reenactments/. The full dialogue-conversations from which the seeds were retrieved from are found in full-conversations/ which also has audio for the entire sequence of reenactments created by the reenactors.

All audio is in 16KHz format. The stimuli, seeds, reenactments, and reenactment files are all mono. All other audios are stereo.

metadata/judge-data.xlsx contains the ID, gender, and age range of all 9 participants. metadata/source-conversations.xlsx contains information on each speaker in the seeds including their ID and the source conversation, the names of the source recordings, track, corpus name, and the URL for the corpus from which the source conversations were taken. metadata/reference-conversations.xlsx contains information on the reenactors including an ID, the names of their full reenactment recordings, gender, age range, and initials.
