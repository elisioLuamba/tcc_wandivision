README – TCC Wandivision
Sistema de Monitoramento Ergonômico Industrial com YOLOv8 Pose

Sistema de monitoramento corporal desenvolvido em Python, utilizando inteligência artificial para identificar posturas e gerar alertas ergonômicos em tempo real.

Configurado para funcionar em computadores sem placa gráfica dedicada (GPU), utilizando processamento pela CPU.

1. Pré-requisitos
Windows 10/11, Linux ou macOS.
Anaconda ou Miniconda instalado.
Python 3.10.
Webcam USB ou integrada.
Mínimo de 4 GB de RAM (recomendado 8 GB).
Conexão com internet para instalação das bibliotecas e download do modelo.
2. Criar o ambiente Conda

Abra o Anaconda Prompt ou terminal e execute:

bash
conda create -n tcc_wandivision python=3.10 -y


Ative o ambiente:

bash
conda activate tcc_wandivision

3. Instalar PyTorch para CPU

Como o projeto será executado sem GPU NVIDIA, instale a versão para processamento pela CPU:

bash
conda install pytorch torchvision cpuonly -c pytorch -y

4. Instalar as bibliotecas

Execute:

bash
pip install ultralytics opencv-python numpy


Bibliotecas utilizadas:

Ultralytics: execução do YOLOv8 Pose.
OpenCV: captura da webcam e processamento de imagens.
NumPy: cálculos matemáticos e distâncias corporais.
PyTorch: processamento do modelo de inteligência artificial.
5. Estrutura do projeto
text
TCC_WANDIVISION/
│
├── trabalho.py
├── yolov8n-pose.pt
└── README.md


O modelo yolov8n-pose.pt será baixado automaticamente na primeira execução, caso não esteja disponível localmente.

6. Executar o sistema

Com o ambiente Conda ativado, execute:

bash
python trabalho.py


O sistema inicializará a webcam e carregará o modelo YOLOv8 Pose.

7. Funcionalidades
Detecção corporal em tempo real.
Identificação de pontos-chave do corpo humano.
Monitoramento de postura sentada.
Identificação de mãos na cintura.
Contagem do tempo das posturas.
Alerta de imobilidade após 10 segundos.
Alerta de sobrecarga após 10 segundos.
Dashboard com interface visual roxa e rosa.
8. Encerrar o sistema

Pressione a tecla:

text
Q

9. Executar novamente

Sempre que abrir o projeto, utilize:

bash
conda activate tcc_wandivision
python trabalho.py

10. Observação

O sistema utiliza processamento pela CPU, não sendo necessária uma placa gráfica NVIDIA ou instalação de CUDA.

O desempenho dependerá da capacidade do processador, da memória RAM e da resolução utilizada pela webcam.

Projeto desenvolvido para fins acadêmicos – Trabalho de Conclusão de Curso (TCC).
