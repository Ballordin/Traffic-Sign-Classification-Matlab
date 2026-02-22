# Classificação de Sinais de Trânsito em Tempo Real 🛑

Este projeto foi desenvolvido no âmbito da unidade curricular de **Robótica** da licenciatura em Engenharia Eletrotécnica e de Computadores (IPCA). O sistema utiliza visão computacional para detetar e classificar sinais de trânsito através de uma webcam em tempo real.

## 🎯 Objetivos
- Implementar algoritmos de processamento digital de imagem em **MATLAB**.
- Desenvolver uma Interface Gráfica (GUI) interativa para controlo e calibração.
- Validar o desempenho do sistema através de métricas de precisão e recall.

## 🛠️ Tecnologias e Ferramentas
- **Linguagem:** MATLAB
- **Toolboxes:** Image Acquisition Toolbox, Image Processing Toolbox.
- **Hardware:** Webcam integrada/USB.

## ⚙️ Metodologia Técnica
O pipeline de processamento de imagem segue estas etapas:
1. **Aquisição:** Captura de frames em tempo real.
2. **Pré-processamento:** Conversão do espaço de cor RGB para **HSV** (para maior robustez à iluminação).
3. **Segmentação:** Aplicação de thresholds dinâmicos para isolar as cores do sinal (Vermelho, Azul).
4. **Morfologia:** Operações de erosão e dilatação para remoção de ruído.
5. **Extração de Características:** Análise de propriedades geométricas (circularidade, centroides e bounding boxes).
6. **Classificação:** Lógica baseada em regras para distinguir sinais como STOP, Sentido Obrigatório, etc.

## 📊 Resultados e GUI
A aplicação (App Designer) permite ao utilizador:
- Ajustar os limites de cor (H, S, V) em tempo real através de sliders.
- Visualizar a máscara binária e o resultado da classificação sobreposto ao vídeo.
- Gerar um histórico de validação para cálculo de estatísticas de acerto.


---
© 2026 Tiago Oliveira - Engenharia Eletrotécnica @ IPCA
