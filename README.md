# BotScheduler

A class used to simplify the scheduder of complex function.

## Usage:

```python 
from schedulerbot import bot

def pipeline():
    print("Hello World!")


logspath = "./logs/"
cachdir = "./cache/"
deltatime = 60 * 60 * 24
start_hour = 10
start_minutes = 30
bot = Bot(logspath, cachdir, deltatime=deltatime)
bot.operations = pipeline
bot.run(start_hour, start_minutes)

```