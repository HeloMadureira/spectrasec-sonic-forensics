
---

# 📡 SPECTRASEC

### Análise Forense de Sinais e Sonificação de Dados

## 🧾 Visão Geral do Projeto

Este repositório documenta uma **Prova de Conceito (PoC)** voltada à **Segurança Ofensiva, Criptoanálise e Forense Digital**.

O objetivo do projeto é demonstrar como a **sonificação de dados binários** pode ser utilizada como **ferramenta forense complementar**, permitindo a identificação de:

* Criptografia
* Ofuscação
* Esteganografia
* Anomalias em fluxos de dados

Em vez de analisar apenas representações hexadecimais ou estatísticas, o projeto converte a **entropia dos dados em frequências de áudio**, possibilitando que o analista **ouça a estrutura interna** de um arquivo e identifique se ele está limpo, criptografado ou alterado.

---

## 🎧 Demonstração – Análise de Áudio

A seguir estão amostras de áudio geradas pelo algoritmo.
📌 Recomenda-se o uso de **fones de ouvido** para melhor percepção das diferenças na textura sonora.

---

### ▶️ Arquivo 1: `radio_hackeado.wav`

**(Raw / Encrypted)**

**O que você vai ouvir:**
Ruído branco denso, estática contínua e ausência de padrões audíveis.

**Diagnóstico Técnico:**
A alta entropia sonora indica dados **fortemente criptografados ou ofuscados**.
A inexistência de padrões repetitivos é característica de **cifras seguras** ou sinais interceptados com alto nível de interferência.

---

### ▶️ Arquivo 2: `radio_limpo.wav`

**(Decrypted / Recovered)**

**O que você vai ouvir:**
Presença de padrões rítmicos, oscilações regulares ou harmônicos perceptíveis.

**Diagnóstico Técnico:**
A redução da entropia auditiva indica que a criptografia foi removida e que o **payload original foi recuperado**.
A estrutura sonora confirma a existência de **dados logicamente organizados e legíveis**.

---
---

## 📊 Evidência Visual – Análise de Amplitude e Bits

A imagem abaixo ilustra uma análise pericial baseada na variação de amplitude do sinal, evidenciando a modificação de bits em nível LSB (Least Significant Bit).

![Análise Forense de Amplitude e Bits LSB](images/laudo_pericial_lsb.png)

📌 **Interpretação Forense**  
As alterações discretas na amplitude, imperceptíveis ao ouvido humano, indicam a presença de dados embutidos no sinal de áudio. Esse tipo de modificação é característico de técnicas de **esteganografia sonora**, utilizadas para ocultar informações em fluxos aparentemente legítimos.

---

## 🛠️ Arquitetura Técnica

O projeto foi desenvolvido em **Python**, utilizando bibliotecas de **Processamento Digital de Sinais (DSP)** para converter bytes em ondas **PCM (Pulse-Code Modulation)**.

A metodologia aplicada envolve conceitos de:

* **Engenharia Reversa**
  Análise estrutural de dados binários

* **Análise Espectral**
  Visualização e audição da densidade e distribuição de entropia

* **Criptografia e Ofuscação**
  Comparação entre dados cifrados e dados recuperados

---

## 🎯 Objetivo do Projeto

Demonstrar que o **som pode ser utilizado como vetor analítico**, ampliando a capacidade de detecção forense além das abordagens tradicionais baseadas apenas em código, logs ou estatísticas.

---

## 👩‍💻 Autoria

**Heloísa Madureira Figueiredo**
Cybersecurity Researcher & Developer

---

