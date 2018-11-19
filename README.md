# timeFormatting
Getting time between past date and future timespan.

# Syntax
  ```
  on load:
    set {x} to 3
    set {y} to 6
    set {_now} to now
    subtract numToTimespan({x}, "hour") from {_now}
    subtract numToTimespan({y}, "day") from {_now}
    set {_result} to getBetweenFormatted({_now}, now)
    send "%{x}% saat ve %{y}% gün = %{_result}%" to console
    set {_calc} to getBetweenTime({_result}, 9 days)
    send "9 gün ve %{_result}% arasındaki zaman farkı: %{_calc}%" to console```
