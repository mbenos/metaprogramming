# Prisoner's Dilema Exploration

Your task is to continue our group-coding activity from the first lecture.
Implement a Prisoner class that has the following methods:

 - `__init__(self, both_confess_sentence, none_confess_sentence, self_confess_sentence, other_confess_sentence)`
 - `decide(self)`
 - `sentence(self, years)`

It doesn't matter what you call your prisoner class (funny names are acceptable).
However, call your file `"<computing id>_prisoner.py"`

Your submissions will compete at the beginning of next class. Extra credit for the winner *and* the looser.

 ### __init__

`__init__` takes in the sentence (penalty in years) for each of the four scenarios as parameters in the following order:

 - Both prisoners confess and rat on eachother
 - Both prisoners keep their mouths shut and don't confess
 - `self` confesses but the other prisoner doesn't
 - the other prisoner rats `self` out, but `self` didn't confess!

`__init__` needs to take in these parameters in order to make informed decisions about whether  to confess.

### decide

The `decide` method takes in no parameters other than `self`. It should decide whether to confess or to remain silent.
It should return `True` to confess and `False` to keep quiet.

### sentence

The `Sentence` method takes in a sentence in years. You may assume that this sentence is associated with the previous decision.
The prisoner will probably want to remember this sentence somehow so that he/she can make a more informed decision next time.