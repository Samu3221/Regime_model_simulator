Here everything about the simulator will be explained and the simulator setting for the figures will be stated.

The Simulator has 3 versions. Taking the following inputs which will be explained from where it stands.

It will also be explained which value needs to be used it is important to state most setting need to be the same for the seed to work.

It also needs to be understood that the simulator uses plotly for live plotting allowing the user to see the boundaries sadjust in real time.

Version 1:

extreme_event_probability_historical:float
extreme_event_probability_forward:float
lamb:float
historical_drift_scalar:float
forward_drift_scalar:float
seed:int
regime_lookBack:int 

Simulator(extreme_event_probability_historical = Chance of an extreme jump occuring in the historical price path, mostly used to model goals in a game ,
              extreme_event_probability_forward = chance of an extreme jump occuring in the forward price path, mostly used to model goals in a game,
              lamb = What the lambda is,  can be understood in the paper what it's function is, shortly explained it widens or narrows the boundaries NEEDS TO BE ABOVE 0
              historical_drift_scalar = How much drift the historical price path needs to have,
              forward_drift_scalar = How much drift the foreward price path needs to have,
              seed = seed is used to specify the randomness from the numpy module.
              regime_lookBack = How far the regime look back time needs to be in stpes. cant be above the historical steps
              

Version 2:

extreme_event_probability_historical:float
extreme_event_probability_forward:float
lamb:float,historical_drift_scalar:float
forward_drift_scalar:float
seed:int
regime_lookBack:int
historical_steps:int
forward_steps:int
tick_time_seconds:float
wallet_value:int
fill_probability:float
with_wallet: bool
        
Simulator(extreme_event_probability_historical = Chance of an extreme jump occuring in the historical price path, mostly used to model goals in a game ,
              extreme_event_probability_forward = chance of an extreme jump occuring in the forward price path, mostly used to model goals in a game,
              lamb = What the lambda is,  can be understood in the paper what it's function is, shortly explained it widens or narrows the boundaries NEEDS TO BE ABOVE 0
              historical_drift_scalar = How much drift the historical price path needs to have,
              forward_drift_scalar = How much drift the foreward price path needs to have,
              seed = seed is used to specify the randomness from the numpy module.
              regime_lookBack = How far the regime look back time needs to be in stpes. cant be above the historical steps
              historical_steps = Used to specify how many steps or ticks needs to be taken in the historical price path,
              forward_steps = Used to specify how many steps or ticks needs to be taken in the Forward price path,
              tick_time_seconds = time per tick, it can be lowered or highed depending on if it it is wished to observe the boundaries slow or fast,
              wallet_value = start value of the wallet ,
              fill_probability = probability of the order selling and buying thus making the wallet increase or decrease in value ,
              with_wallet = weather to display wallet path or not
Version 3:

Simulator(extreme_event_probability_historical = Chance of an extreme jump occuring in the historical price path, mostly used to model goals in a game ,
              extreme_event_probability_forward = chance of an extreme jump occuring in the forward price path, mostly used to model goals in a game,
              lamb = What the lambda is,  can be understood in the paper what it's function is, shortly explained it widens or narrows the boundaries NEEDS TO BE ABOVE 0
              historical_drift_scalar = How much drift the historical price path needs to have,
              forward_drift_scalar = How much drift the foreward price path needs to have,
              seed = seed is used to specify the randomness from the numpy module.
              regime_lookBack = How far the regime look back time needs to be in stpes. cant be above the historical steps
              historical_steps = Used to specify how many steps or ticks needs to be taken in the historical price path,
              forward_steps = Used to specify how many steps or ticks needs to be taken in the Forward price path,
              tick_time_seconds = time per tick, it can be lowered or highed depending on if it it is wished to observe the boundaries slow or fast,
              wallet_value = start value of the wallet ,
              fill_probability = probability of the order selling and buying thus making the wallet increase or decrease in value ,
              historical_VarAndVol_lookback = How many steps historical price paths variance and volatility needs to be taken as input into the startign boundaries, ,
              with_wallet = weather to display wallet path or not
