=============================
Dataset
=============================

===============  ============  =========  ========  ====================================  =======================
Dataset Name     Type          #Samples   # Hours   Task                                  Metrics
===============  ============  =========  ========  ====================================  =======================
MDRM-test [1]       Short Clips   22,208     87        short financial clip ASR              WER
SPGISpeech-test [2]  Short Clips   39,341     130       short financial clip ASR              WER
Earning-21 [3]       Long Audio    44         39        long financial audio ASR              WER
Earning-22 [4]       Long Audio    125        120       long financial audio ASR              WER
FinAudioSum      Long Audio    64         55        long financial audio Summarization    Rouge-L & BERTScore
===============  ============  =========  ========  ====================================  =======================


We create *FinAudioSum* based on the ECTSum dataset, originally designed for earnings call summarization using textual data. ECTSum comprises 2,425 earnings transcripts paired with expert-generated, telegram-style summaries. We obtain corresponding audio recordings for the ECTSum test set from `earningscast <https://earningscast.com/>`_. Overlapping recordings with Earnings-21 and Earnings-22 (spanning 2019–2022) are removed. The final *FinAudioSum* dataset includes 64 recordings totaling 55 hours.

[1] [What You Say and How You Say It Matters: Predicting Financial Risk Using Verbal and Vocal Cues](https://aclanthology.org/P19-1038.pdf) ACL 2019. [Data](https://github.com/GeminiLn/EarningsCall_Dataset/tree/master)
[2] [SPGISpeech: A Large-Scale Dataset for Financial Speech Recognition](https://arxiv.org/pdf/2104.02014) InterSpeech 2021.
[3] [Earnings-21: A practical benchmark for ASR in the wild](https://arxiv.org/pdf/2104.11348) InterSpeech 2021.
[4] Earnings-22: A Practical Benchmark for Accents in the Wild