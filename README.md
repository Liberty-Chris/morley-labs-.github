![alt text](https://github.com/Morley-Labs/morley-docs/blob/main/branding/morley.png)

# **Morley** – A Ladder Logic Based Language for Smart Contracts on Cardano

**ArkWriter is evolving. Things will break. There is much work to do.**

**Morley** is a domain-specific language (DSL) that brings **Ladder Logic programming** to **Cardano Smart Contracts**, enabling automation engineers, industrial programmers, and IoT developers to build **blockchain-powered automation** with ease.

By compiling Ladder Logic into **Plutus Core**, **Morley** simplifies smart contract development for those familiar with **PLC programming**, **embedded systems**, and **industrial automation**.

## **Why Morley?**
- **Industry-Friendly** – Designed for engineers in **IoT, manufacturing, and automation**.
- **Faster Development** – Write Cardano smart contracts in an intuitive Ladder Logic syntax.
- **Blockchain Integration** – Secure, verifiable transactions on Cardano.
- **Transparency & Auditability** – Track machine states, events, and industrial processes.
- **Efficient & Lightweight** – Optimized for **on-chain execution**.

## **Use Cases**
**Morley** enables **trustless** and **automated** decision-making in industries such as:
- **Industrial Automation** – Log sensor data, trigger smart actions on the blockchain.
- **Supply Chain & Logistics** – Track inventory and automate contractual agreements.
- **Energy Management** – Secure monitoring of power grids and resource allocation.
- **Aerospace & Automotive** – Machine error tracking, predictive maintenance, and quality assurance.
- **IoT & Embedded Systems** – Secure communication between connected devices.
- **Decentralized Finance (DeFi)** – Machine-driven DeFi actions (e.g., automatic staking or lending).

## **Project Components**
| Component                 | Description                                     |
|---------------------------|-------------------------------------------------|
| **LadderCore**            | Intermediate representation (IR) for Ladder Logic |
| **LL-Parser**             | Parses Ladder Logic into IR                    |
| **PlutusLadder Compiler** | Compiles IR into Plutus Core                   |
| **PlutusLadderSim**       | Simulates Ladder Logic in a blockchain environment |

## **Getting Started**
### 1️⃣ Installation
(to be continued)

### 2️⃣ Example Smart Contract
A **Ladder Logic-based Smart Contract** that tracks an **inventory system** on **Cardano**:

```
(* Define Inputs and Outputs *)
X1   --[ ]----------------( )-- Counter1 (* Item scanned in inventory *)
X2   --[ ]----------------( )-- Counter2 (* Item removed from inventory *)

(* Trigger a blockchain event when threshold is reached *)
Counter1 == 100  --[ ]--( )-- TX_Send(* Mint new tokens when inventory is full *)
Counter2 == 0    --[ ]--( )-- TX_Send(* Burn tokens when inventory is empty *)

(* Implement a reset condition *)
Reset --[ ]--( )-- Counter1 (* Reset inventory counter *)
Reset --[ ]--( )-- Counter2 (* Reset removed items counter *)
```

### 3️⃣ Compile to Plutus Core
To compile the smart contract to Plutus Core, run the following command:

```bash
morley compile contract.ll
```

## 🎨 Morley GUI - ArkWriter
The **Morley GUI** is a simple interface for building Ladder Logic-based smart contracts. Designed with usability and clarity in mind, the GUI simplifies complex workflows without overwhelming the user. Extended functionality is in progress.

![alt text](https://github.com/Morley-Labs/morley-docs/blob/main/branding/arkwriter_logo_multi-use.png)

![alt text](https://github.com/Morley-Labs/morley-docs/blob/main/ArkWriter_Screens/Screenshot%202025-02-09%20210231.png)

![alt text](https://github.com/Morley-Labs/morley-docs/blob/main/ArkWriter_Screens/Screenshot%202025-02-09%20210326.png)

![alt text](https://github.com/Morley-Labs/morley-docs/blob/main/ArkWriter_Screens/Screenshot%202025-02-09%20210356.png)

![alt text](https://github.com/Morley-Labs/morley-docs/blob/main/ArkWriter_Screens/Screenshot%202025-02-09%20210344.png)

![alt text](https://github.com/Morley-Labs/morley-docs/blob/main/ArkWriter_Screens/Screenshot%202025-02-09%20210446.png)

[Learn more at morleylang.org](https://morleylang.org)

## 📖 Documentation
Visit our Documentation Hub to explore:

- **Advanced Tutorials**
- **Smart Contract Deployment**
- **Best Practices for Blockchain Integration**
- **Industry-Specific Research**

## 🤝 Contributing
We welcome contributions from developers, industrial engineers, and blockchain enthusiasts. If you'd like to contribute:

1. **Fork a repository**.
2. **Create a feature branch**:  
```bash
git checkout -b feature/your-feature
```
3. **Submit a pull request**:  
Open a pull request to share your work with the community and contribute to the Morley project!

## 💡 License
This project is licensed under the **APACHE 2.0 License**. Feel free to use and adapt **Morley** to your needs while crediting the original authors.

## 🌐 Stay Connected
- **Website**: [morleylang.org](https://morleylang.org)  
- **X**: [@morleycardano](https://x.com/morleycardano)

