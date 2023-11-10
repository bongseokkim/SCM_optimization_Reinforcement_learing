# SCM_optimization_Reinforcement_learing
SCM_optimization using Reinforcement learing

# Adaptive Supply Chain Management Using Reinforcement Learning

## Abstract
Supply chain management capability is a critical component directly connected to a company's competitiveness. Traditional research methods assume that customer demand is known in advance through statistical distribution and that it remains stable (stationary), approximating solutions through various optimization techniques. However, in the real world, customer demand is unknown and varies over time, presenting clear limitations. This study aims to find adaptive supply chain management policies through reinforcement learning, defined as a Markov decision process. The problem is solved using policy-based reinforcement learning algorithms. The optimal policy proposed in this study is expected to yield about 9-24% increased profits compared to the traditional inventory management model of Economic Order Quantity (EOQ). The supply chain modeled in this study is composed of factories, factory warehouses, and distribution warehouses, forming a 1:1:N connection relationship. It is assumed that the flow of goods is unidirectional. The agent must decide on the production quantity at the factory to maximize profit and how much to send from the factory warehouse to the distribution warehouse. Subsequent chapters detail the assumed demand patterns in the MDP configuration and the terms used in Tables 1, 2, and 3.

## Supply Chain Configuration
The supply chain consists of three types: the factory, the factory warehouse, and the distribution warehouse, with a 1:1:N connection relationship. It is assumed that the flow of goods is unidirectional. 

## Demand Patterns
Demand patterns are divided into three major types: Constant, Linear drop, and Seasonality, with uniform random noise added to each to conduct experiments in a total of six scenarios. The agent cannot observe the current demand and must decide how much to produce and how much to distribute to the warehouses based on uncertain past demand information.

## MDP Definition
The agent's observed state includes all warehouse inventory levels at time t and information on past demands. The state consists of two types of information: inventory levels at the factory and distribution warehouses and observed patterns of past demands. 

## Actions and State Transitions
The agent's actions are two-fold: determining the production level at the factory and the amount of goods to be shipped to the distribution warehouse. The state transition is defined as the next state occurring from the current inventory level, demand, and action.

## Results
The experimental results compare the proposed approach against the fixed-order quantity (EOQ) method over six demand patterns. The algorithm used is the Twined Delayed DDPG (TD3), a type of policy-based reinforcement learning algorithm. The supply chain network used for the comparison is a simple 1:1:1 network.

## Conclusion
The agent achieved higher profits than the EOQ model, especially in terms of storage costs, by producing only as needed and minimizing unnecessary inventory.

---

For more detailed information on the methodology, results, and implications of this study, please refer to the full paper.

## Figures and Tables
- Figure 2: Supply Chain Configuration
- Table 1: Symbol Definition for Factory
- Table 2: Symbol Definition for Factory Warehouse
- Table 3: Symbol Definition for Distribution Warehouse
