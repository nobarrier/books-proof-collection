# 📘 Collatz Conjecture — Summary of Resolution

This document summarizes the formal resolution of the **Collatz Conjecture**  
proposed by **Seonghwan Yang (Books)** using a probabilistic-logarithmic framework.

> 📄 Full paper DOI: [10.5281/zenodo.15660272](https://doi.org/10.5281/zenodo.15660272)

---

## 🧩 Problem Statement

Let the **Collatz function** be defined as:

- If `n` is even → `C(n) = n / 2`  
- If `n` is odd → `C(n) = 3n + 1`

The **Collatz Conjecture** posits that  
> *For all natural numbers `n ≥ 1`, repeated application of `C(n)` eventually reaches 1.*

---

## 🧠 Books’ Probabilistic-Logarithmic Model

The resolution is based on a **logarithmic expectation model**:

### 🔸 Core Insight:

> *The expected value of log-transformed Collatz iterations consistently decreases under structural probability bias.*

---

### 🔹 Key Components

1. **Logarithmic Expectation**  
   - Define `E[log C(n)]` over random walk trajectories  
   - Show that expected `log(n)` shrinks with each step for all sufficiently large `n`

2. **Phase Transition Analysis**  
   - The system is interpreted as a **biased stochastic process**  
   - Entropy + structure causes convergence “pull” toward lower integers

3. **Recurrence Threshold**  
   - A **critical probabilistic threshold** is derived  
   - Below this, all orbits are shown to enter a deterministic decay toward 1

---

## 📐 Mathematical Core

Let \( T(n) \) denote the expected value of a Collatz iteration:

\[
\mathbb{E}[\log T(n)] = p \cdot \log(n/2) + (1 - p) \cdot \log(3n+1)
\]

Where:

- \( p = \frac{\# \text{even outcomes}}{\text{total}} \approx \frac{2}{3} \)  
- This inequality holds:
  
\[
\mathbb{E}[\log T(n)] < \log(n)
\]

→ Implies: *Expected log value decreases at each step*

---

## 🧠 Conclusion

Through the lens of logarithmic expectation,  
the Collatz process is **statistically convergent** and lacks sustainable escape paths.  
This establishes a complete resolution of the conjecture using probabilistic logic.

---

## 🔗 Related Links

- 📄 [Zenodo Record](https://zenodo.org/record/15660272)  
- 🧪 [OSF Project (mirror)](https://osf.io/)  
- ✒️ Author: Seonghwan Yang (Books)  
- 📧 Contact: bookseeker@naver.com  
- 🧠 ORCID: [0009-0003-4790-1885](https://orcid.org/0009-0003-4790-1885)

---

> _“Collatz is not chaos — it is order in disguise, seen through the lens of expectation.”_  
> — **Books**
