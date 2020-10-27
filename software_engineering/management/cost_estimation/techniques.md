# Techniques for cost estimation

1. Expert Judgement
   * Several experts on the proposed technique and application estimate project cost. There are discussed and compared until an agreement is reached.
   * Some expert judgement techniques involve polling each expert independently, in some cases for three estimates, pessimistic \(p\); optimistic \(o\) and most likely \(m\).

     Then estimate is computed by e = \(p + 4m + o\)/6

   * Delphi technique: asks several experts to make an individual judgement of the effort using any method they wish. Then, the average effort is calculated, and presented to all of the experts.

     Each expert is given a chance to revise, discussion maybe involved. This process repeats until a concensus has been reached.
2. Estimation by analogy
   * The cost of a new project is estimated based on similar projects in the same application domain. 
3. Parkinson's Law
   * This law states the work will fill the time available.
   * The cost is determined by available resources than by objective assessment. 
   * For example, if the software is to be delivered in 12 months, and 3 people are available, the effort is 36 person months.
4. Pricing to win
   * The cost is estimated to be whatever the customer has available to spend on the project. cost depends on budget not functionality.
5. Algorithmic cost modelling
   * A model is developed using historical cost information based on some software metric \(usually its size\) to the project cost. 
   * When a project effort needs to be estimated, an estimate of the metric is computed. 
   * Using the model, effort is predicted.
   * The most general form is := Effort = A _Size^B_ M

     where

     ```text
     A is a constant factor based on organisational practices.
     Size is the size of the software estimated in a metric of choice.
     B is a value between 1 and 1.5 derived experimentally. 
     M is a multiplier made by combining various attributes (process, stability of reqs, experience, skill).
     ```

