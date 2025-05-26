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

- `join_mapping.csv`: Maps each new utterance ID to one or more original segments from the LibriHeavy corpus
- ESPnet2 asr1 directory structure (KALDI based)

## 🧪 Use Case

This dataset is useful for:

- Training and Evaluating long-form ASR (consistent sets available in multiple versions based on different average segment durations)
- Studying error propagation in long audio
- Testing new segment joining and resegmentation strategies

## 📎 Citation

Coming soon.

## 📄 License

Released under the [MIT License](LICENSE).
