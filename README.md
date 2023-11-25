# A Corpus of Pragmatic-Similarity Judgments over Spoken-Dialog Utterances
This is a collection of pragmatic-similarity judgments of spoken-dialog utterance pairs. There were two data collection sessions done with english(EN) stimuli and one session done with spanish(ES) stimuli. The first EN session had 1,980 pragmatic-similarity judgments, the second EN session had 1,872, and the ES session had 1,410. Judgments are done on a continuous scale of 1 to 5, where 1 represents no similarities between an utterance pair and 5 represents two utterance pairs that are almost identical. Each pair consists of a seed, taken from a real dialog, and a reenactment, separated by a beep. The reenactments were created using 6 methods described in a conference paper that is under preparation.

## Expected Uses
This data is intended to be used on training an automatic model of similarity.

## Collection Procedure
Judgments were collected in four hour judgment sessions where there where 6-9, mostly naive, judges in one room. The judges were trained on the rating process and then listened to the stimuli and gave judgments. Judgments were entered using a QuestionPro form: https://utepsubacc.questionpro.com/t/AX8ttZzJBn.

## Directory Structure and File Formats
The judgment-data/ directory has the excels with the pragmatic-similarity judgments for 689 stimuli. Each row has columns for the stimulus #, stimulus name, seed name (Source1), and reenactment name (Source2), as well as the judge IDs and the judgments given by them. The seeds are named with the clip-source code and the clip #. The reenactments are named with the method used, the re-enactor code, and the seed name. The stimuli are named with a randomly assigned number, assigned in a reordering of the stimuli, an F that signified the stimuli was complete, and the reenactment name, which already has the seed name.

The stimuli used in the judgment sessions are found in EN-stimuli-reordered/ and ES-stimuli-reordered/ as well as the kids stimuli used found in EN-kids-stimuli/ and ES-kids-stimuli/. There are a total of 458 EN stimuli, 10 EN kids stimuli, 230 ES stimuli, and 5 ES kids stimuli. We were not able to do some methods for two seeds due to missing context required for those reenactment methods. We only used 689 stimuli across all three judgment sessions. The seed utterances chosen for creating the stimuli are found in EN-seeds/ and ES-seeds/, while the reenactments of those utterances are found in EN-reenactments/ and ES-reenactments/. The full dialogue-conversations from which the seeds were retrieved from are found in EN-full-conversations/ and ES-full-conversations/, which also have the audio for the entire sequence of reenactments created by the reenactors.

All audio files are mono and 44.1KHz format. The only exception are audio files in full-conversations/ where the source convsersations are all stereo and either 16KHz or 8KHz format, and the reenactment audios are mono and 16KHz format.

metadata/judge-data.xlsx contains the ID, gender, and age range of all 12 judges that participated.

metadata/EN-source-conversations.xlsx and metadata/ES-source-conversations.xlsx contains information on each speaker in the seeds including their ID and the source conversation, found under clip-source code, it also has the names of the source recordings, track info, corpus name, and the URL for the corpus from which the source conversations were taken. metadata/EN-reference-conversations.xlsx and metadata/ES-reference-conversations.xlsx contains information on the reenactors including an ID, the names of their full reenactment recordings, gender, age range, and initials.
