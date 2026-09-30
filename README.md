# 🗺️ GURPS Travel Time Calculator

A focused Java desktop utility to calculate overland travel times, march rates, and distances for **GURPS 4th Edition**.

---

## 📖 Overview

Designed to streamline overland exploration logistics during tabletop sessions, this project bridges practical GMing needs with hands-on practice in **Java**. 

By automating the math behind movement rates, the tool allows GMs and players to quickly evaluate daily travel limits or determine the exact time required to traverse specific distances across an adventure map.

---

## 📐 Mechanics & House Rules

In standard **GURPS 4th Edition** rules, ideal daily march distance is calculated as:

$$\text{Daily Distance (miles)} = \text{Basic Speed} \times 10$$

In actual table play, multiplying by 10 often assumes optimal paved roads, perfect clear weather, and continuous marching without interruptions—which rarely reflects adventuring reality. Conversely, a flat multiplier of 5 (commonly cited across community forums) can overly penalize parties by assuming constant harsh conditions.

To strike a balanced, realistic middle ground for typical wilderness expeditions:

* **Implemented Multiplier:** This tool calculates daily pace using a baseline of **$\text{Basic Speed} \times 7$ miles/day**.
* **Total Time Calculation:** Determines total travel days by dividing target distance by the calculated daily pace.

---

## ✨ Features

* **Daily Distance Mode:** Enter a character's **Basic Speed** and click **Calculate Distance** to retrieve their daily march capacity in miles.
* **Duration Mode:** Provide a target distance in miles (alongside Basic Speed) to calculate total days needed for the journey.
* **Input Validation:** Enforces the dependency of distance calculations on the character's Basic Speed stat.

---

## 🛠 Tech Stack

* **Language:** Java (JDK 17+)
* **GUI Toolkit:** JavaFX / Swing *(ajuste conforme o toolkit usado)*
* **Build Tool:** Maven / Gradle

---

## 🗺️ Roadmap

- [ ] Implement **Hiking skill** bonuses and modifiers
- [ ] Add terrain type multipliers (swamp, mountain, jungle, desert)
- [ ] Add weather condition modifiers (heavy rain, snow, extreme heat)
- [ ] Support mounted travel and pack animal movement rates
- [ ] Add forced march fatigue tracking

---

## 🚀 Getting Started

### Prerequisites

* Java Development Kit (JDK) 17 or higher installed

### Running Locally

```bash
# Clone the repository
git clone [https://github.com/your-username/gurps-travel-calculator.git](https://github.com/your-username/gurps-travel-calculator.git)
cd gurps-travel-calculator

# Compile and run
javac Main.java
java Main
