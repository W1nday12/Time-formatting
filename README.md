Until now, you have only printed time in one format.

import datetime as dt


arrival_time = dt.datetime(2019, 5, 10, 19, 45)
print('Plane arrives at', arrival_time) 
The plane arrives at 2019-05-10 19:45:00 
What should you do if you want to type a message in a human way, say: It's 10:31? 
There is a strftime() method for this.
It can be applied to any datetime object and the argument can be used to specify the time output format:
print('Plane arrives at', arrival_time.strftime('%H:%M')) 
The plane arrives at 19:45 
Here %H means hours, %M means minutes. 
In addition to these parameters,
there are also,
for example,
%B - month,
%Y - year and %S - seconds,
%A - name of the day of the week in English,
%U - week number in the year.
