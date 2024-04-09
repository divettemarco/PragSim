# A Corpus of Pragmatic-Similarity Judgments over Spoken-Dialog Utterances
This is a collection of judgments of the pragmatic-similarity between 689 dialog-style utterance pairs.

## Expected Uses:
This data is intended to be used on training an automatic model of similarity.

## Motivation:
While automatic measures of similarity between utterances are invaluable --- for training speech synthesizers, evaluating machine translation, and assessing learner productions --- and there exist measures for semantic similarity and prosodic similarity, there were none for pragmatic similarity, nor any resources for training or evaluating them.

## Stimuli:
Each pair consists of a seed, taken from a real dialog, and a reenactment. The reenactments were created using 6 methods, chosen to obtain pairs with a variety of degrees of similarity.

## Instrument:
Judgments are on a continuous scale of 1 to 5, where 1 represents no similarity between the utterances and 5 represents two utterances that are pragmatically almost identical.

## Judges and Procedure:
Each pair was judged by 6 to 9 subjects, mostly naive, in one room. The judges were trained on the rating process and then listened to the stimuli and gave judgments. This happened in three judgment sessions, each lasting four hours, with all judges synchronously and independently making judgments, and entering them using a QuestionPro form.

## Data Size:
There were two data collection sessions with English (EN) stimuli, and one session with Spanish (ES) stimuli. There are a total of 458 adult EN stimuli, 10 child EN stimuli, 230 adult ES stimuli, and 5 child ES stimuli. Across all judges, the first EN session yielded 1,980 pragmatic-similarity judgments, the second EN session 1,872, and the ES session 1,410.

## Directory Structure and File Formats:
The judgment-data/ directory has excel spreadsheets with the pragmatic-similarity judgments for all 689 stimuli. Each row has columns for the stimulus #, stimulus name, seed name (Source1), and reenactment name (Source2), as well as the judge IDs and their judgments. The seed names include the clip-source filename and the clip number. The reenactments names include the method used, the re-enactor code, and the seed name. The stimuli are named with a randomly assigned number, assigned to govern the order of presentation, the letter F to signify that this was a finalized stimulus, and the reenactment name, which also contains the seed name.

Most of the audio stimuli themselves are found in EN-stimuli-reordered/ and ES-stimuli-reordered/, with the remainder being the stimuli from young children, which is in EN-kids-stimuli/ and ES-kids-stimuli/. The seed utterances are in EN-seeds/ and ES-seeds/, and the reenactments in EN-reenactments/ and ES-reenactments/. To support per-speaker normalizations, the full conversations from which the seeds were extracted are available in EN-full-conversations/ and ES-full-conversations/, as are the recordings for each re-enactor's entire sequence of reenactment attempts.

All audio files are .wav files, variously in mono and stereo, and variously in 44.1KHz, 16KHz and 8KHz.

The metadata/ directory includes judge-data.xlsx contains the ID, gender, and age range of all 12 judges that participated. It also includes EN-source-conversations.xlsx and ES-source-conversations.xlsx, which list information on each speaker in the seeds including their ID and the source conversation information, including the source recording filenames, track, corpus name, and the URL for each source corpus. It also includes EN-reference-conversations.xlsx and ES-reference-conversations.xlsx, which contain information on the re-enactors, including an ID, the names of their full reenactment recordings, gender, age range, and initials.

More information is in A Collection of Pragmatic-Similarity Judgments over Spoken Dialog Utterances. Nigel G. Ward and Divette Marco. LREC-COLING 2024.
