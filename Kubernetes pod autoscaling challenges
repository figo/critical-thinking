Three key challenges still exist in Kubernetes pod autoscaling: 
1. users tend to reserve more resources than necessary; 
2. parameters requires continuously fine-tuning; 
3. the learning curve is steep

At #intuit kubernetes team, we developed a comprehensive recommendations engine for auto scaling parameters 
and a recommendation synthesizer and applier that enables zero-configuration auto scaling for users. 
We plan to open-source all pieces in the future.

The pod size recommender analyzes 7+ days of historical metrics to provide stable and 
optimized pod CPU and memory recommendations. 

The recommendation synthesizer generates the final recommendation by ingesting both vertical 
and horizontal recommendations. The applier further refines the recommendation with safeguards, 
such as only reducing a small percentage when reducing size, reaching the desired size through 
multiple iterations, and verifying and compensating during each iteration.
