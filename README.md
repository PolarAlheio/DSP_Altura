# DSP_Altura
Sistema de medição de altura utilizando visão computacional e OpenCV.

# Estimativa de Altura Humana com Calibração ArUco

Este projeto implementa um sistema de **estimativa de altura humana** usando uma **webcam** e **processamento digital de imagens (DSP)**.  
A técnica se baseia na detecção de um **marcador ArUco de tamanho conhecido**, que serve como referência para converter medidas em pixels para metros.

O sistema realiza:
1. Captura de um **frame do fundo** (sem pessoa).
2. Captura de um **frame com a pessoa** posicionada.
3. **Subtração de fundo** para isolar o corpo.
4. Aplicação de **filtro gaussiano** e **limiarização** para melhor detecção de contornos.
5. Detecção automática do **marcador ArUco** e cálculo da escala.
6. Estimativa da **altura da pessoa em metros** com base no tamanho do contorno principal.

---

## Contexto
Trabalho desenvolvido para a disciplina **Processamento Digital de Sinais (DSP)**, com foco em **processamento de imagens e visão computacional**.

---

## Tecnologias Utilizadas
- **Python 3.10+**
- **OpenCV 4.10.0**
- **NumPy**
- **cv2.aruco** 
- **Webcam**

---
