# Student describes the effect of the P, I, D component of the PID algorithm in their implementation. Is it what you expected?

## Proportional component:
The Proportional component directs the vehicle towards the centerline proportionally to the cte. With only the P component, the car tends to overshoot and oscillate over the centerline.
## Integral component:
The Integral component works to cancel out steering drift, bringing the vehicle closer to the centerline the longer it is away from the centerline.
## Derivative component:
The Derivative component relates the derivative of the cte, meaning that the closer the vehicle gets to the centerline, the less of an attack angle it has, slowly meeting the centerline. this reduces oscillation.

# Student discusses how they chose the final hyperparameters (P, I, D coefficients). This could be have been done through manual tuning, twiddle, SGD, or something else, or a combination!

I manually picked and tried different coefficients from open online sources. I then tuned it a little based on the behavior of it. Mostly the D coefficent to reduce the oscillation.

