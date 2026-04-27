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




# InSeC: Steganysis Model Based on Inter-codeword Sensitivity Caption for Compressed Speech Streams
Official PyTorch implementation of InSeC (IEEE Access 2024) — A high-accuracy, real-time, and robust steganalysis model for Joint Parallel Steganography (JPS) detection.

---

## ✨ Highlights
- 🚀 **The first dedicated model for JPS steganalysis** in compressed VoIP speech.
- 📈 **SOTA performance** under extremely low embedding rates (1%–9%).
- 🛡️ **Strong anti-packet-loss ability** (still effective at 5%–20% packet loss).
- ⚡ **Real-time inference**: Only 2.39 ms per 1-second speech.
- 🌐 **Supports Chinese & English datasets**, compatible with G.729.
- 🧪 **Full experiments reproducible**: ablation, embedding rate, duration, packet loss.

---

## 📌 Model Overview
InSeC uses a two-stage architecture:
1. **Steganography-sensitive Codeword-pair Caption Module (SCM)**: Captures multi-view sensitive changes of codeword pairs.
2. **Fine-grained Correlation Re-perception Module (FCRM)**: Refines local feature dependencies.

It accurately detects CNV, PSR, and JPS steganography.

---

## 📊 Performance
| Metric | Result |
| :--- | :--- |
| Avg Accuracy Gain | +8% vs. existing methods |
| 1% Embedding Rate | 50.42% (CN) / 50.89% (EN) |
| 20% Packet Loss | >81% accuracy |
| Speed | 2.39 ms / 1s speech |

---

## 📂 Project Structure
