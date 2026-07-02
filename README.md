### 📌 Framework Note
This repository is developed based on an open-source Genetic Programming for Job Shop Scheduling (GPJSS) benchmarking framework built upon the Java ECJ library. The original package structure and foundational scheduling simulation modules have been retained, while this repository introduces the extension for multi-tree representations, continuous task transitions, and surrogate-assisted lifelong learning mechanisms proposed in the submitted manuscript.

# Surrogate-Assisted Lifelong Genetic Programming for Dynamic Flexible Job Shop Scheduling

This repository provides the official implementation of the Surrogate-assisted Lifelong Genetic Programming (LLSGP) framework for automated design of dispatching rules in Dynamic Flexible Job Shop Scheduling (DFJSS).

The package is built upon the Java-based ECJ (Evolutionary Computation in Java) framework, specifically tailored for multi-tree representations, continuous learning across dynamic environments, and efficient surrogate models to prevent catastrophic forgetting.

---

## 🛠️ Environment Setup & Dependencies

1. **Prerequisites:** * Java JDK 11 or higher.
    * IntelliJ IDEA (recommended project environment).

2. **Project Structure Realignment:**
    * Ensure that the core algorithmic source files in the `src/` folder and external library dependencies (e.g., Apache Commons Math, ECJ core files) are fully loaded in your IDE project build path.
    * If using IntelliJ IDEA, simply set the project root directory as the **Content Root** and mark the `src/` folder as **Sources Root**.

3. **Code Modules:**
    * `src/ec/`: Core ECJ foundational framework functions.
    * `src/yimei/jss/`: Domain-specific packages for Job Shop Scheduling, containing dispatching rule representations, discrete event simulation environments, and tree evaluation models.

---

## 📂 Key Architecture Modifications

The core components of the proposed lifelong learning and surrogate mechanisms are located within `/src/yimei/jss/algorithm/lifelongGP/`:

---
## 🚀 Running Experiments: Launching the Proposed Lifelong GP

1. Locate the target parameter configuration file:
   `src/yimei/jss/algorithm/lifelongGP/multipletreegp-dynamic.params`
2. Run the main class `src/yimei/jss/gp/GPRun` with the following command-line argument:
   ```bash
   -file src/yimei/jss/algorithm/lifelongGP/multipletreegp-dynamic.params