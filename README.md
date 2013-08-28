state_machine forked from [pluginaweek/state_machine](https://github.com/pluginaweek/state_machine)

### Changelog:

A hash with ```  {name: :state_name, value: state_value}  ``` can be passed in initial.

### Why?

In previous implementation 

```
  class Bike

    PARKED  = 0

    state_machine attribute: :status, :initial => :parked do
      state :parked, value: Bike::PARKED
    end

  end
``` 
would initialize with status "parked"