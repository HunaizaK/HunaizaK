<h1 align="center">Hunaiza Khan</h1>

<p align="center">
  <b>Machine Learning Engineer</b> · AI Engineer at SIRP · AI &amp; Data Science Trainer
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/hunaiza-khan197/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-Hunaiza%20Khan-0A66C2?style=flat-square&logo=linkedin&logoColor=white"></a>
  <a href="mailto:hunaizakhan197@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-hunaizakhan197%40gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white"></a>
</p>

---

I build **production ML and LLM systems**, from data and modelling to evaluation, compression and a served API. My priorities are honest metrics and finding out *why* a model fails.

-  **AI Engineer at SIRP**, building ML and LLM systems that run in production.
-  **Trainer:** I teach a 12-week AI & Data Science course to about 40 students at Ashrei Tech (NASTP), and I'm a section leader for **Stanford's Probability for AI** course.
-  **Research:** probabilistic flood forecasting for Pakistan (*FLARE*, below).
-  **Currently exploring:** model compression for deployment, calibration and uncertainty, and evaluating LLM systems.

## Featured projects

Every number below comes from a real run recorded in the repo. Each repo has tests, pinned dependencies, a FastAPI service where relevant, and an error-analysis section.

| Project | What it does | Result |
|---|---|---|
| [**text-classification-nlp**](https://github.com/HunaizaK/text-classification-nlp) | News topics: TF-IDF + SVM vs fine-tuned **DistilBERT**, then **int8 quantization** and **distillation** | 90.2% vs 88.0% (p = 0.0006); int8 model **268 → 139 MB**, 1.7× batch throughput; distilled linear student 89.4% |
| [**image-processing-classical-vs-deep**](https://github.com/HunaizaK/image-processing-classical-vs-deep) | Traffic signs (GTSRB): OpenCV **HOG + SVM** vs a Keras **CNN**, with corruption-robustness tests | CNN 97.7% vs 94.5%; on rotated signs **64% vs 14.5%**; classical model 0.66 MB at 1.1 ms/image |
| [**customer-churn-ml**](https://github.com/HunaizaK/customer-churn-ml) | Telecom churn: segmentation, 4-model comparison, **cost-based decision threshold**, SHAP explanations | ROC-AUC 0.845; tuned threshold catches **88% of churners** at **10% lower** expected cost |
| [**deep-learning-architectures**](https://github.com/HunaizaK/deep-learning-architectures) | Nine architectures implemented, trained and analysed: feed-forward, CNN (Keras + PyTorch), LSTM/GRU, **transformer from scratch**, VAE, DCGAN, SimCLR | CNN 90.5% on Fashion-MNIST; transformer from scratch 83.8% on IMDB; whole suite runs in 23 min on CPU |
| [**ipcv**](https://github.com/HunaizaK/ipcv) | Elderly-care monitoring: real-time action detection with an **X3D-M 3D CNN**, alert smoothing, caregiver email alerts, React dashboard | 78.9% on people never seen in training; **100% of falls and staggering** caught |
| [**Adaptive-E-learning-Platform**](https://github.com/HunaizaK/Adaptive-E-learning-Platform) | RL tutor (**DQN vs PPO**) that sequences 73 Python lessons over an 18-concept prerequisite graph | Showed that the top-reward agent (DQN, 2.3× the fixed curriculum's reward) was **gaming the reward**: 19.4 prerequisite violations per session |

<table>
  <tr>
    <td align="center" width="33%">
      <a href="https://github.com/HunaizaK/image-processing-classical-vs-deep"><img src="https://raw.githubusercontent.com/HunaizaK/image-processing-classical-vs-deep/main/reports/figures/preprocessing.png" alt="HOG feature pipeline on a dark traffic sign"></a>
      <br><sub>Contrast equalisation and HOG edges on a dark traffic sign</sub>
    </td>
    <td align="center" width="33%">
      <a href="https://github.com/HunaizaK/deep-learning-architectures"><img src="https://raw.githubusercontent.com/HunaizaK/deep-learning-architectures/main/dcgan/results_full/samples.png" alt="DCGAN samples"></a>
      <br><sub>DCGAN samples after 40 epochs</sub>
    </td>
    <td align="center" width="33%">
      <a href="https://github.com/HunaizaK/customer-churn-ml"><img src="https://raw.githubusercontent.com/HunaizaK/customer-churn-ml/main/results/shap_beeswarm.png" alt="SHAP churn drivers"></a>
      <br><sub>SHAP explanations of what drives churn</sub>
    </td>
  </tr>
  <tr>
    <td colspan="3" align="center">
      <a href="https://github.com/HunaizaK/image-processing-classical-vs-deep"><img src="https://raw.githubusercontent.com/HunaizaK/image-processing-classical-vs-deep/main/reports/figures/robustness.png" alt="Robustness of CNN vs HOG+SVM under image corruptions"></a>
      <br><sub>Robustness test: CNN vs HOG + SVM accuracy as noise, blur, darkness, rotation and occlusion increase</sub>
    </td>
  </tr>
</table>

## Research

**FLARE: probabilistic river-discharge forecasting and flood mapping, Jhelum and Indus basins.** A single LSTM serves 13 river gauges and outputs a full distribution for each forecast day, not just one value. Satellite-radar (Sentinel-1) thresholds then turn each forecast into a flood map.

- **Average R² of 0.818** across 13 stations and 7 days ahead (0.916 one day ahead).
- **Flood-map F1 up to 0.969.**
- Deployed in a disaster-response platform for shelters, incident reports and donations.

*H. Khan, F. Shahid, S. M. Awan, NED University of Engineering and Technology.*

## Teaching

- **AI & Data Science, a 12-week course** at Ashrei Tech (NASTP), about 40 students, starting from Python and NumPy.
- **Section leader, Stanford's Probability for AI.**

## Tech stack

**ML & deep learning**
<br>
<img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white">
<img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white">
<img alt="Keras" src="https://img.shields.io/badge/Keras-D00000?style=flat-square&logo=keras&logoColor=white">
<img alt="TensorFlow" src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white">
<img alt="scikit-learn" src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white">
<img alt="LightGBM" src="https://img.shields.io/badge/LightGBM-2C7BB6?style=flat-square">
<img alt="Stable-Baselines3" src="https://img.shields.io/badge/Stable--Baselines3-RL-555555?style=flat-square">

*Classical ML · CNNs · RNNs/LSTMs · transformers · generative models · reinforcement learning · distillation & quantization*

**NLP, vision & LLMs**
<br>
<img alt="Hugging Face" src="https://img.shields.io/badge/Hugging%20Face-Transformers-FFD21E?style=flat-square&logo=huggingface&logoColor=black">
<img alt="OpenCV" src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white">
<img alt="PyTorchVideo" src="https://img.shields.io/badge/PyTorchVideo-EE4C2C?style=flat-square&logo=pytorch&logoColor=white">

**Data**
<br>
<img alt="pandas" src="https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white">
<img alt="NumPy" src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white">
<img alt="SQL" src="https://img.shields.io/badge/SQL-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white">
<img alt="Google Earth Engine" src="https://img.shields.io/badge/Google%20Earth%20Engine-4285F4?style=flat-square&logo=googleearth&logoColor=white">

**MLOps & backend**
<br>
<img alt="FastAPI" src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white">
<img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white">
<img alt="GitHub Actions" src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white">
<img alt="pytest" src="https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white">
<img alt="React" src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB">
<img alt="Streamlit" src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white">


---

<p align="center">
  <sub>Open to ML engineering conversations: <a href="https://www.linkedin.com/in/hunaiza-khan197/">LinkedIn</a> · <a href="mailto:hunaizakhan197@gmail.com">hunaizakhan197@gmail.com</a></sub>
</p>
