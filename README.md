![VBB_Thumbnail_1280x720](https://github.com/user-attachments/assets/4e1e22df-85a6-4587-9451-49a7d8bd6d8a)

# Online Learning Project 2023-24
This project implements a dynamic online learning framework designed to optimize pricing campaigns using advanced techniques such as multi-armed bandits, UCB (Upper Confidence Bound) strategies, and discretization approaches. The goal is to develop a policy that efficiently learns the optimal bidding strategies over time by balancing exploration (gathering information) and exploitation (using known information to maximize rewards).

The framework is suitable for environments where bidders participate in auctions or pricing campaigns, where decisions need to adapt dynamically based on the observed feedback.

## Requirements
- 🟢 **Requirement 1**: Stochastic Environment: distribution over the bids of the other agents and a function specifying the probability with which an user buys for every price.
  - Build a pricing strategy using a  **continuous** set of prices p and a **Gaussian Process**
  - Consider a sequence of second-price auctions. Build two learning algorithms to deal
    with the bidding problem:
    - A primal-dual algorithm for truthful auctions
    - A UCB-like algorithm
- 🟢 **Requirement 2: adversarial environment**: Build an highly non-stationary environment. At an high level, it should include:
  - A sequence of competing bids of the other agents (e.g., sampled from a
    distribution that changes quickly over time)
  - For each day, a function specifying the probability with which an user buys for
    every price (this function changes quickly over time)
  - Consider a generalized first-price auction. Build a learning algorithms to deal with
    the bidding problem. In particular, a primal-dual algorithm for non-truthful auctions.
- 🟢 **Requirement 3: two extensions for pricing**:We extend the pricing problem along two directions. Since we focus only on pricing, we directly consider a demand curve with noise (di↵erently from previous points in which the demand curve depends on the number of visits and hence on the advertising step).
  - Build a non-stationary environment for the pricing problem. At an high level:
    - Days are partitioned in intervals
    - In each interval the demand curve is di↵erent
    - The demand curve + noise specifies how many buyers while buy for every price
      depending on the current interval
  - Build a pricing strategy using the discretization of the prices p 2 [0, 1] and:
    - **sliding-window**
    - **CUSUM**
- 🟢 **Requirement 4: Compare di↵erent bidding algorithms**: The goal is to compare the performances of di↵erent algorithms.
Consider the di↵erent algorithms that we have seen for bidding and let them play one
against the others in a generalized first-price auction. In particular, consider:
  - A primal-dual algorithm for truthful auctions
  - A primal-dual algorithm for non-truthful auctions
  - A UCB-like approach

## Results
16 points out of 16

## Contributors

[Margherita Brogi](https://github.com/margheritaaa10)

[Alfonso Shytani](https://github.com/AlfiSHY)

[Luca Trizio](https://github.com/lucatrizio)

## Credits
Thanks to [Think With Google]([https://mpost.io/glossary/game-theory/](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.thinkwithgoogle.com%2Fintl%2Fen-emea%2Fmarketing-strategies%2Fautomation%2Fbidding-for-value-automation%2F&psig=AOvVaw2RR7UhwSc6YvArzMFf5M-3&ust=1728465212320000&source=images&cd=vfe&opi=89978449&ved=0CBcQjhxqFwoTCICW_Yme_ogDFQAAAAAdAAAAABAE)) for the header image
