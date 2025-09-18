\# 🌐 X-Pay Documentation (English)



\[X-Pay](https://www.x-pay.fun/) is an open-source \*\*multi-chain cryptocurrency payment system\*\* that provides secure, scalable, and developer-friendly payment solutions for merchants, developers, and Web3 applications.



\## 🚀 Key Features

\- Multi-chain \& Multi-token Support: Currently supports TRON (TRC-20 USDT), planned support for ETH, BSC, etc.  

\- Unified Architecture: Generalized table structure and modular design for easy extension to new chains and tokens.  

\- Automatic Fund Collection: Address pool management + mnemonic-based addresses with automated consolidation.  

\- Real-time Monitoring: Transaction and address monitoring via TronGrid / Web3 RPC with instant callbacks.  

\- Developer Friendly: RESTful API \& SDKs (Java / Node.js / Frontend), backend built with Spring Boot + MyBatis Plus.



\## 📦 Tech Stack

\- Backend: Spring Boot 3, MyBatis Plus, RxJava, Web3j, Tron Java SDK  

\- Frontend: Vue 3 (Tailwind), deployed on Cloudflare Pages  

\- Database: MySQL



\## 🔧 Getting Started

1\. Clone the repository:

```bash

git clone https://github.com/x-pay-official/x-pay.git

cd x-pay

```

2\. Configure environment (database, blockchain RPC, API keys)  

3\. Start the service:

```bash

./mvnw spring-boot:run

```



\## 🏗 Architecture Overview

```mermaid

flowchart TD

&nbsp;   User\[User] --> |Initiates Payment| Merchant\[Merchant System]

&nbsp;   Merchant --> |Creates Order| XPay\[X-Pay Service]

&nbsp;   XPay --> |Assigns Deposit Address| Wallet\[Address Pool]

&nbsp;   User --> |Sends Payment| Wallet

&nbsp;   Wallet --> |Monitors Transactions| XPay

&nbsp;   XPay --> |Sends Callback| Merchant

```



\## 📎 Related Repositories

\- x-pay-java-sdk — Java SDK  

\- x-pay-node-sdk — Node.js SDK  

\- x-pay-vue-demo — Vue frontend demo  

\- x-pay-react-demo — React frontend demo



\## 📌 Roadmap

\- Support ETH / BSC USDT  

\- Launch enhanced auto-collection module  

\- Multi-tenant SaaS support  

\- Add webhook signature verification \& replay protection



\## 🤝 Contributing

Contributions welcome via PRs or Issues. Please follow CONTRIBUTING.md guidelines.



\## 🔗 Links

\- Website: https://www.x-pay.fun/  

\- GitHub Org: https://github.com/x-pay-official



