# stattlepy

Stattleship PYTHON Wrapper brought to you by [@stattleship](https://twitter.com/stattleship).

Check out the [Stattleship API](https://www.stattleship.com) - The Sports Data API you've always wanted

Affordable. Meaningful. Developer-Friendly.

:football: :basketball: and :black_circle: with :baseball: coming soon. 

We're gonna need a bigger :boat:!

## Differences From R API wrapper

Due to '''type''' function in python, to indicate the type of stat you would like to query, use the '''stat_type''' variable in the API call 

## Install
With pip:
```
pip install git+https://github.com/ashleyhansberry/stattleship-python
```

## Getting Started
Obtain an access TOKEN from [stattleship.com](www.stattleship.com). Load Python and initialize your TOKEN for your session and load the library:

```
from stattlepy import Stattleship
New_query = Stattleship()
Token = New_query.set_token('YOUR_TOKEN')
Output = New_query.ss_get_results(sport='basketball',league='nba',ep='game_logs',player_id='nba-stephen-curry')
```

## Getting Results
Reference the [Developer API](http://developers.stattleship.com) for information on all the types of commands that can be formatted. In general, the sport=, league=, ep= portions of the ss_get_results call correspond to the end portion of the HTTP Request URL. 

