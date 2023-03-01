# FAQ

## Design

---

### Q) Why did your team decide to launch Factorial on Polygon?

- 60% of DeFi TVL stays in Ethereum Network, but more than 90% locked in EVM compatible blockchains. Factorial platform works best within the environment where lots of DeFi protocols exist to connect with, so it was our timely decision to build as set of EVM compatible contracts.

- Moreover, majority of retail users are more active on L2, especially on Polygon. Therefore, our team decided to launch Factorial on Polygon first, and then expand to other L2, EVM chains and Ethereum Network.

- In far future, we believe this status will change over time. More DeFi activities will be diversified to other ecosystem outside EVM world, and we will slowly prepare for expansion of our service outside EVM world.

### Q) Factorial is not a just simple code but a combination of modules and ecosystems. What kind of modules consist of?

| Valuation Module : Connects oracle services to calculate value of any DeFi positions in Factorial | Liquidation Module : Manages liquidation process requested by apps built on Factorial |
| --- | --- |
| Asset Management Module : Interfacing users/apps for risk check of changes requested from apps/users | Connector Module : Relays requests of execution  at external DeFi protocols from apps |

### Q) FTR staking holder will get their reward by the proportional fee on Factorial. Is there any specific fee structure?

- FTR staker community will decide by governance how much of the fee accumulated from Factorial module interactions will be distributed to FTR stakers as protocol fee.

- Most importantly, services which create higher probability of larger amount of risk exposure to Factorial and its users will be the multiplier of protocol fee proportion.

### Q) Is there any specific tokenomics of FTR? (e.g., inflation, token distribution, burning mechanism)

- There are two categories of ecosystem participants:
    - Resource Providers
        - providing resources for the ecosystem, such as oracle services, liquidators, market makers, liquidity providers, app developers, insurers
        - they will receive incentives calculated from resource they provided for the ecosystem
    - Utility Consumers (Users)
        - end-users consuming utilities provided by resource providers
        - they will pay fee/tax related to their corresponding utilities they consumed
- FTR token stakers will have the governance rights to decide revenue distribution

## Security

---

### Q) How Factorial check sanity of changes requested by each app built on Factorial?

- In principle, any change occurring on assets owned by users should not result in significant financial damages. Asset Management module does sanity check on every request transaction from users/apps so that we can make sure it does not cause any significant loss to users.

- This is possible by utilizing Valuation module which is responsible for external data feeding and conservative asset valuation with configuration decided by governance. Exceptions of financial loss allowed are from slippages or liquidation costs, which are executed by Factorial modules.

### Q) Why multi-DeFi apps built on Factorial are more secure than stand-alone apps?
    
There are several reasons why apps built on Factorial are much safer than stand-alone apps:
    
- Rather than re-inventing wheels for widely duplicated financial functions for each stand-alone apps, developers can simply call functions provided by Factorial modules to significantly reduce the codebase
    - minimized codebase is much easier for auditors or community to audit.
    - less codebase means lower risk of bugs and backdoor codes.
    - app developers do not need significant funding to create an innovative DeFi.
  
- Infrastructure around newly developed DeFi can be shared by Factorial ecosystem
    - Infrastructure such as oracles, liquidators, lenders, auditors, potential users, and even frontend services can be shared from Factorial ecosystem, so that the app developers do not need to invest efforts to build those infrastructure.
    - Because an integrated ecosystem is stronger than scattered infrastructure by each stand-alone apps, Factorial will provide much deeper ecosystem to be used by apps.
  
- Single user interface through Factorial modules
    - Every communication with end-users is handled by Asset Management module in Factorial, which does not allow for newly developed apps on Factorial to phish or manipulate user’s messages.
    - Also, Asset Management module does sanity check for every transaction coming into Factorial to make sure the apps are not requesting something which might damage user’s asset significantly.
  
- Factorial is a public goods to be used and reviewed by many ecosystem participants
    - Because Factorial serves its functionalities to wide range of users including app developers and DeFi end users, it is also their needs to verify that the functions provided by Factorial are securely developed and operated. Hence, Factorial framework will be stronger over time with the growth of Factorial’s ecosystem which cannot be competed with stand-alone app’s infrastructure over long run.
     
- Factorial team is best suited for technologically&financially secure platform development
     - Our team has been accumulating teamwork capability for almost 5 years, with balanced talents from financial industry and blockchain engineering. We know how to design economically viable DeFi apps, and also know how to build secure apps for blockchain community. We have experience on how to grow community, partnerships and ecosystem for DeFi apps.

- Q) When we assume that tremendous apps are integrated/built on factorial, Is there any risk-hedging strategy in the case of an unexpected hack or critical issue on the Factorial module itself?
    - very strict and throughout testing and simulation process for internal development cycle.
    - slow and infrequent upgrade of modules to minimize risk exposure on changes of codes.
    - economically and structurally conservative approach to have various limits in the modules so that the amount of exploitation risk is capped even in the bug existing situation.
    - frequent audits by multiple auditors to minimize vulnerabilities within Factorial modules.
    - bug bounty alive for bug hunters to recognize and fix potential risk factors.

## Ecosystem

---

### Q) What components make up the Factorial Ecosystem?

- **Oracle Services** : connected with Valuation module to serve external on-chain/off-chain data for valuation of DeFi assets within Factorial.

- **Liquidators and Market Makers** : participates in liquidation process via Liquidation module to resolve financial situation and reduce risk.

- **App Developers** : represents new creative multi-DeFi applications to be deployed and served for DeFi users in Factorial ecosystem.

- **DeFi Users** : provides or consumes resources or services operated on Factorial and interact each other within the integrated ecosystem.

### Q) What kind of initial multi-DeFi apps/use cases on Factorial are needed?

- Team will build 3 multi-DeFi apps in-House:
    - Lending : becomes a bank to lend tokens not only to individuals but also to whitelisted apps built on Factorial.
    - DeFi Leverage : collateralizing user’s assets including DeFi positions to allow DeFi leveraging, borrowing tokens from Lending app.
    - Managed Fund : a passive investment tool for DeFi investors to allow restricted control of users’ aggregated fund by professional fund managers.

- Other than above, we expect more variety of multi-DeFi apps such as list below will attract users:
    - Margin Trading : margin trading without tokens by collateralizing DeFi positions
    - P2P OTC : allows any individual to easily create a financial contract each other by collateralizing their DeFi positions
    - Synthetic Assets : creating derivatives products such as option products utilizing Factorial’s given features
    - Automated Fund Management : automated trading service with pre-defined strategy for passive investment tools

### Q) How can you attract creative multi-DeFi app developers into Factorial ecosystem?

- Because app developing experience on Factorial will be similar to learning a new smart contract language, it is very important for us to educate developers so that they can fully understand how Factorial modules should be used to build apps on Factorial.

- Documents and Contents
    - We will provide very explanative documents to understand how to utilize Factorial modules to build different kinds of multi-DeFi applications.
    - We will frequently publish blog posts and video contents where developers can learn about Factorial modules and its use-cases.

- Frequent Events
    - There will be very frequent hackathons for potential app developers to incentivize research and experience on Factorial to grow our developer community.

- Study Courses
    - We will provide study courses to acquire necessary information about Factorial modules to allow students to have consistent motivation and acquire knowledge.

### Q) There are so many sectors factorial need to build from the ecosystem perspective, what is your expected first external ecosystem partner? (Starting point of the ecosystem)

- Initial B2B partnerships will be focused on oracle services and liquidators.

- For oracle service, Chainlink will be one of the main partnership, but we will have additional oracle service providers to diversify risk of oracle manipulation.

- For liquidators, there will be several partnerships with market makers to make sure multiple competition on liquidation auction process to minimize difference from fair value and liquidated value. B-Harvest will also participate in this process to make competition tighter.

## Competition

---

### Q) What projects are your competitors in this market and what’s the big difference between Factorial?

- Multi-DeFi platform such as Instadapp is the only competitor of Factorial with similar purpose. But its platform does not provide fully modular functionalities for building new DeFi apps, but simply connecting multiple DeFi protocols to automate asset management. However, Factorial’s vision allows multi-DeFi developers to build their own creative logic utilizing Factorial modules, significantly reduce overhead to re-inventing wheels for core financial functionalities and infrastructure building. Therefore the vision and depth of modularity and functionality of each platform is very different.

- Multi-DeFi apps such as Alpha Homora, Yearn Finance, 1Inch Exchange are competitors for the apps built on Factorial. Those apps will compete with existing services by sharing modules and ecosystem provided by Factorial to create stronger and more secure infrastructure than stand-alone applications.

### Q) As an inherently unique product, why has no other succeeded in doing what Factorial plans to do?

- In traditional finance, when we trade stocks, we don’t directly interface with exchanges. We interface with brokers who connect multiple exchanges and financial products around the world to provide convenient one-stop gateway.

- But in DeFi, the phase of the industry is in early days, and most builders are focusing more on building stand-alone applications(more like “infrastructure” in tradFi) than seamless gateway for convenient user experience.

- However, this gateway should not be operated in a centralized way because it will destroy the strength of DeFi primitive, trustless and transparency. And it is not easy for builders to design such platform to trustlessly connect with various DeFi and provide modules for creating new interconnected utilities.

- After significant growth in DeFi since summer 2020, it is the right time for us to provide such platform to greatly enhance user’s convenience and utility to accelerate again the mass adoption of DeFi.

### Q) Is the Expected Valuation for Factorial realistic? How did you come up with the number?

- Current total DeFi TVL is about $50B. We believe that when Factorial is successful, a lot of popular multi-DeFi apps will be built and operated on Factorial platform. Even though Factorial apps are not directly possessing assets, it is the Factorial ecosystem which possess interfaces with end-users, hence value accrual for such user-base and TVL is stronger on platform side than each products utilized from platform.

- Because Factorial ecosystem will acquire end-users, the potential valuation of Factorial is much larger than many existing stand-alone DeFi protocols combined.

- However, because Factorial is challenging the new norms for DeFi ecosystem, the valuation is heavily discounted to only 0.2% of total DeFi TVL, $100M.
