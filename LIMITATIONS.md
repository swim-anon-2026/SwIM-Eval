# Limitations

**Corpus scope and resource bias.**  
The current evaluation covers three corpora (Bangor Miami, Bangor Siarad, Bangor Patagonia) that predominantly feature higher-resource languages (English, Spanish, Welsh). While typologically varied, results may not fully generalize to low-resource code-switching scenarios with greater OOV rates and data scarcity. Extending SwIM to low-resource CS corpora remains important future work.

**Model coverage and architectural evolution.**  
Four distinct ASR architectures are considered; however, the rapid pace of multilingual ASR means newer or specialized models may introduce behaviors not captured here. Ongoing benchmarking is needed to maintain relevance.

**Pilot scope and methodological refinement.**  
An initial pilot was limited to 20 samples from a single corpus, adequate for surfacing pipeline issues (e.g., temporal alignment) but not for fully optimizing the Contextual Window (W). A larger, dedicated study is required to empirically tune W across diverse language pairs.

**Human evaluation and perceptual alignment.**  
This release does not include a direct comparison between SwIM scores and human perception of transcription quality within contextual windows. Establishing this correlation is a priority for future work to connect SwIM’s localized error diagnosis with user experience.
