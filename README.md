# 🎓 Monitoramento de Alunos em Tempo Real

![Machine Learning](https://img.shields.io/badge/Machine%20Learning-TensorFlow-orange)
![Computer Vision](https://img.shields.io/badge/Computer%20Vision-OpenCV-blue)
![Python](https://img.shields.io/badge/Python-3.12-green)
![Notebook](https://img.shields.io/badge/Environment-Colab-yellow)

---

## 📝 Descrição do Projeto

Protótipo de **monitoramento e reconhecimento em tempo real de alunos** através de imagens do rosto, utilizando **aprendizado de máquina** e **visão computacional**.

O sistema captura imagens da câmera do notebook, extrai **embeddings faciais** e compara com um banco de dados previamente treinado para identificar os alunos em tempo real.

**Problema resolvido:**  
Em instituições de ensino, a presença e a atenção dos alunos são informações importantes, mas o monitoramento manual é demorado e sujeito a erros. Esta aplicação automatiza o processo, permitindo **identificação rápida e confiável** de cada aluno.

---

## 🛠 Tecnologias Utilizadas

- 🟠 **TensorFlow / Keras** – Treinamento e inferência de modelos de reconhecimento facial.  
- 🔵 **OpenCV** – Captura de vídeo e processamento de imagens.  
- 🐍 **Python 3.12** – Linguagem principal do projeto.  
- 💻 **Google Colab** – Ambiente de desenvolvimento e teste do protótipo.  

---

## 🏛 Arquitetura do Sistema

```text
┌───────────────────┐
│ Webcam do Notebook│
└────────┬──────────┘
         │ Captura imagens
         ▼
┌───────────────────┐
│ Pré-processamento │
│ - Redimensionamento│
│ - Normalização    │
└────────┬──────────┘
         │
         ▼
┌───────────────────┐
│ Modelo de CNN /   │
│ Face Embeddings   │
└────────┬──────────┘
         │
         ▼
┌───────────────────┐
│ Banco de Embeddings│
│ de Alunos         │
└────────┬──────────┘
         │ Comparação / Reconhecimento
         ▼
┌───────────────────┐
│ Resultado em Tempo│
│ Real: Aluno ID    │
└───────────────────┘
