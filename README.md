# Introduction

Teacher equipared azure functions as the old web jobs:

![comparing to web jobs](images/comparing-to-web-jobs.png)

There are three consumption plans:

- Consumption;
- Premium;
- Dedicated.

The consuption plan has autoscale (automatic scale). Premium is related to a low latency, integrations. Dedicated is related to the functions that is hardly used. The consumption plan is the most used.

The consumption plan has a default time limit of 5 minutes and a maximum time limit of 10 minutes. The premuim and dedicated plans has a default limit of 30 minutes and no maximum limit.

If the function is not used for a interval of time, it will occur a cold start and the function will need more time to answer.


# Scale behaviour

![scale behaviour](images/scale-behaviour.png)

Azure functions has autoscale, but you can limit the maximum number of instances (*functionAppScaleLimit*).