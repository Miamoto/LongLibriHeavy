# LongLibriHeavy: A New Benchmark for Long-Form ASR

**LongLibriHeavy** is a benchmark dataset designed to evaluate Automatic Speech Recognition (ASR) systems on long-form speech.

🔗 Based on [LibriHeavy](https://github.com/k2-fsa/libriheavy)

## 📂 Dataset Structure

Each split (train, dev, test) contains:

- `data.json`: A JSON file with entries per utterance:
  - `audio_filepath`: Path to the full audio file
  - `start`: Start time of the utterance in seconds
  - `end`: End time of the utterance in seconds
  - `duration`: Duration in seconds
  - `text`: Reference transcription

- `join_mapping.csv`: Maps each new utterance ID to one or more original segments from the LibriHeavy corpus (can be used to stylize the training sets to the desired average!!!)
- ESPnet2 asr1 directory structure (Kaldi inspired)

## 🧪 Use Case

This dataset is useful for:

- Training and Evaluating long-form ASR (consistent sets available in multiple versions based on different average segment durations)
- Studying error propagation in long audio
- Testing new segment joining and resegmentation strategies

**Note: This repository is actively maintained and being updated. Please note that the code and documentation are subject to changes and improvements. We recommend regularly checking for updates and referring to the latest version of the repository for the most up-to-date information.**

## 📎 Citation

Please cite our paper if you use our benchmark. 

```
@inproceedings{longlibriheavy,
    title={{Exploring Linear Variant Transformers and k-NN Memory Inference for Long-Form ASR}},
    author={Carlos Carvalho, Jinchuan Tian, William Chen, Yifan Peng, Alberto Abad, Shinji Watanabe},
    booktitle={Proceedings of the 26th Annual Conference of the International Speech Communication Association (INTERSPEECH)},
    year={2025},
}
```

## 📄 License

Released under the [MIT License](LICENSE).
