# TCC Wandivision – Monitoramento Ergonômico Industrial

Sistema de monitoramento corporal e análise ergonômica em tempo real, utilizando **Inteligência Artificial** e **Visão Computacional** com **YOLOv8 Pose**.

---

## 📌 Sobre o Projeto

Este projeto foi desenvolvido para fins acadêmicos (Trabalho de Conclusão de Curso - TCC) na área de **Inteligência Artificial, Visão Computacional e Ergonomia Industrial**. 

O objetivo principal é monitorar posturas corporais no ambiente de trabalho para auxiliar na prevenção de lesões e melhoria da saúde ergonômica. O sistema processa tudo via CPU, dispensando a necessidade de uma GPU dedicada.

---

## 🛠️ Tecnologias Utilizadas

- **Python 3.10**
- **YOLOv8 Pose** (Ultralytics)
- **PyTorch**
- **OpenCV**
- **NumPy**
- **Conda** (Anaconda / Miniconda)

---

## ✨ Funcionalidades

- [x] Detecção corporal em tempo real por webcam.
- [x] Identificação de postura sentada.
- [x] Detecção de mãos na cintura.
- [x] Contagem contínua do tempo mantido em cada postura.
- [x] Emissão de alertas automáticos após 10 segundos na mesma posição.
- [x] Interface gráfica personalizada com paleta em tons de **roxo e rosa**.

---

## 📋 Requisitos do Sistema

- **Linguagem:** Python `3.10`
- **Gerenciador de ambiente:** Anaconda ou Miniconda
- **Hardware mínimo:**
  - 4 GB de RAM
  - Webcam funcional
  - Processamento por CPU (sem necessidade de GPU NVIDIA dedicada)

---

## 🚀 Instalação e Configuração

Siga os passos abaixo para configurar o ambiente e executar o projeto:

### 1. Criar o ambiente virtual Conda
```bash
conda create -n tcc_wandivision python=3.10 -y
```

### 2. Ativar o ambiente
```bash
conda activate tcc_wandivision
```

### 3. Instalar o PyTorch (Otimizado para CPU)
```bash
conda install pytorch torchvision cpuonly -c pytorch -y
```

### 4. Instalar as demais dependências
```bash
pip install ultralytics opencv-python numpy
```

---

## 💻 Como Executar

Com o ambiente ativado, execute o script principal:

```bash
python trabalho.py
```

> ℹ️ **Nota:** O modelo pré-treinado `yolov8n-pose.pt` será baixado automaticamente na primeira vez em que o projeto for executado.

---

## 📁 Estrutura do Projeto

```text
TCC_WANDIVISION/
│
├── trabalho.py        # Código fonte principal da aplicação
├── README.md          # Documentação do projeto
└── requirements.txt   # Lista de dependências do Python
```

---

## 📝 Observações Gerais

O sistema foi otimizado para rodar em computadores convencionais focando no processamento em tempo real via CPU, permitindo acessibilidade sem a necessidade de placas de vídeo dedicadas.
