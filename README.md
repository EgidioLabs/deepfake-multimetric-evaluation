# Avaliação Multimétrica de Deepfakes

Framework de benchmark para análise comparativa de deepfakes baseados em vídeo, integrando métricas biométricas, perceptuais, estruturais e de consistência temporal para avaliação de identidades sintéticas.

---

## Visão Geral

Este projeto apresenta um pipeline experimental para avaliação multimétrica de vídeos deepfake gerados por técnicas de manipulação de identidade. O framework foi desenvolvido para investigar a relação entre fidelidade visual, preservação biométrica e coerência temporal em cenários de renderização facial sintética.

A metodologia de avaliação combina métricas multimodais de Visão Computacional, proporcionando uma análise abrangente da qualidade dos deepfakes além da avaliação puramente perceptual.

---

## Métricas de Avaliação

O benchmark integra as seguintes dimensões analíticas:

- **Identity Similarity**  
  Análise de similaridade biométrica baseada em embeddings faciais gerados com FaceNet512 via DeepFace.

- **LPIPS (Learned Perceptual Image Patch Similarity)**  
  Métrica de similaridade perceptual alinhada à percepção visual humana.

- **SSIM (Structural Similarity Index Measure)**  
  Avaliação da integridade estrutural entre frames de referência e frames sintéticos.

- **Temporal Identity Consistency**  
  Análise de estabilidade da identidade facial ao longo de frames sequenciais.

- **Temporal Visual Consistency**  
  Avaliação da coerência temporal utilizando similaridade estrutural sequencial entre frames.

---

## Tecnologias e Bibliotecas

- Google Colab
- Python 3.12
- DeepFace
- OpenCV
- PyTorch
- LPIPS
- NumPy
- Pandas
- scikit-image
- Matplotlib
- tqdm

---

## Objetivo Experimental

O framework foi desenvolvido para apoiar investigações acadêmicas e experimentais envolvendo:

- Avaliação de fidelidade de deepfakes
- Análise de preservação de identidade sintética
- Avaliação de coerência temporal
- Análise comparativa entre pipelines generativos
- Estudos de segurança voltados a ataques de personificação sintética

---

## Saídas Geradas

O pipeline gera automaticamente:

- Tabelas comparativas resumidas
- Rankings finais de desempenho
- Análises métricas por frame
- Relatórios CSV para avaliação estatística

---

## Contexto de Pesquisa

Este benchmark foi desenvolvido como parte de um estudo acadêmico focado na avaliação de ataques de engenharia social baseados em deepfakes em ambientes de geração assíncrona de vídeo.
