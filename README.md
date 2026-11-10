TCC Wandivision – Monitoramento Ergonômico Industrial

Sistema de monitoramento corporal utilizando Inteligência Artificial e Visão Computacional com YOLOv8 Pose.

Tecnologias
Python 3.10
YOLOv8 Pose
PyTorch
OpenCV
NumPy
Conda
Funcionalidades
Detecção corporal em tempo real.
Identificação de postura sentada.
Detecção de mãos na cintura.
Contagem de tempo das posturas.
Alertas após 10 segundos.
Interface gráfica em roxo e rosa.
Requisitos
Python 3.10
Anaconda ou Miniconda
Webcam
Computador com mínimo de 4 GB de RAM.
Não necessita de GPU dedicada.
Instalação

1. Criar ambiente:

bash
conda create -n tcc_wandivision python=3.10 -y


2. Ativar ambiente:

bash
conda activate tcc_wandivision


3. Instalar PyTorch para CPU:

bash
conda install pytorch torchvision cpuonly -c pytorch -y


4. Instalar dependências:

bash
pip install ultralytics opencv-python numpy

Executar o projeto
bash
python trabalho.py


O modelo yolov8n-pose.pt será baixado automaticamente na primeira execução.

Estrutura do projeto
text
TCC_WANDIVISION/
│
├── trabalho.py
├── README.md
└── requirements.txt

Observação

O sistema foi desenvolvido para fins acadêmicos (TCC) e funciona utilizando processamento pela CPU, sem necessidade de placa gráfica NVIDIA.

Área: Inteligência Artificial, Visão Computacional e Ergonomia Industrial.
