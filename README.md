# Policy-Gradient-Cartpole-Reinforce-Baseline
Policy Gradient Cartpole Reinforce with Baseline

## Policy Gradient Methods -
 To find optimal policy , we have looked at the action value function q , and asked the question - for every state which action is giving 
 us the maximum q value.

 Now , we look at methods which learn an optimal policy without considering the value function.

 The policy is by the defined as the probability of picking an action 'a' given that we are at state 's'.
 This is denoted by- PI(a|s)

 The policy parametrization is carried out by applying the softmax function over the priority/preference order assigned to each action.

## Policy Gradient Theorem
Policy gradient theorem provides as analytical expression for calculating gradient of the performance measure with respect to
the policy parameter.

It is a remarkable result which states that the gradient of the performance measure with respect to the policy parameters does 
not involve the gradient of the state distribution with respect to the policy parameters, even though the state distribution 
depends on the policy parameter.

## Reinforce with Baseline
In the REINFORCE with Baseline method, a constant value is subtracted from the return. This constant value is dependent on the state.

This makes sure that states with high return values do not end up influencing the policy parameter update.

This constant value is called the baseline.
A common practice is to use the value function itself as the baseline.

This method is also called the Actor-Critic method since the value function is like the critic which evaluates the actor which is the return.

